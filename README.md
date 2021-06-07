# Diamond_energy


version 1.0 2021  

Jonathan M. Goodman, Mengman Wei

A program doing conformational searching for acyclic alkanes on diamond framework

#################################################################

# CONTENTS

1. Release Notes

2. Requirements and Setup

3. Usage


#################################################################

# Release Notes

Diamond_energy is a program to do systematic conformational searching for acyclic alkanes. It is developed based on an assumption that local minima have strcutrues closely resemble diamond lattice, and this should allow us to locate all low energy conformations very fast by varying the structure of the molecule under diamond framework.

The program starts from getting information of the molecule from its InChI as input. The structure of the molecule will then be built within diamond lattice, and all its rotatable bonds will be recognized and recored. And then the program will rotate all rotatable bonds of the molecule under diamond framework one by one, to lists all low-energy conformations and estimate of their energies, approximately in kJ/mol. 

#################################################################

# Requirements and Setup

The script was written in a python 3.6+ environment

All development and testing was done on Linux and MacOS

#################################################################

# Usage

Download the Diamond_energy.py script and direct the system path to its location in terminal. The program is run in terminal.

# Correct Usage Argument
python Diamond_energy.py molecularInChI

# Example Argument - Heptane
python Diamond_energy.py "InChI=1S/C7H16/c1-3-5-7-6-4-2/h3-7H2,1-2H3"

The program will automatically do conforamtional searching for heptane, and the searching process and outcome will be shown in terminal including conformation number, their corresponding dihedral angle values, their energys, the lowest energy conformation's number, the lowest energy conformation's dihedral angle value, the lowest energy conformation's coordinates, the number of conformations with accessible energies.







