This repository contains data and simulation input from the paper:

"Application of ESMACS binding free energy protocols to diverse ligand datasets:Bromodomain-containing protein 4" David W. Wright, Shunzhou Wan, Christophe Meyer, Herman van Vlijmen, Christophe Meyer, Gary Tresadern, and Peter V. Coveney

Preprint DOI: [10.26434/chemrxiv.7327019](https://dx.doi.org/10.26434/chemrxiv.7327019)

What follows is a brief description of the contents

# Naming conventions 

Two models based on different crystal structrues were used to create the simulation starting structures, these are referred to by the PDB ascession numbers - 2oss and 4bjx.

Two ligand datasets are studied in this work, which are designated diverse (DIV) and tetrahydroquinoline scaffold (THQ).

- DIV dataset is labelled J1-J12, this coresponds to ligands 1-11 in the paper (with J12 being the second pose of ligand 11).

- THQ dataset is labelled G1-G16.

The naming reflects the origin of the datasets as coming from collaborations with Janssen and GSK respectively.

# Directories

## initial-pdbs

Contains the PDBS used to create starting structures, including conserved water molecules

## ligand-ff-params

Forcefield files (`frcmod` and `prep`) describing parameterized ligands.

- `am1` - contains AM1-BCC parameters for the DIV ligands
- `gauss` - contains all ligands parameterized using Gaussian/RESP method

## mmpbsa

Files related to MMPBSA analysis in tab separated values format.

- `input` - contains the MMPBSA input file used for all analyses
- `2oss` and `4bjx` - contain results for the two different starting structures

Within the two results directories sub-directories contain results calculated with differing numbers of explicit water molecules, labelled `watX` with `X` indicating the number of water molecules.

## simulated-topologies

Amber forcefield topology (`prmtop`) and coordinate (`inpcrd` and `pdb`) files for all ligand for both the `2oss` and `4bjx` structures.

[![DOI](https://zenodo.org/badge/156712132.svg)](https://zenodo.org/badge/latestdoi/156712132)
