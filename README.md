# HapSolo2

HapSolo2 is an AI optimization approach designed for the removal of secondary haplotigs in diploid genome assembly and scaffolding processes. The method employs a forward-looking randomized hill-climbing algorithm, integrating AI techniques, to minimize the cost associated with genomic assemblies. 

HapSolo2 is coded completely in Python, and libraries used include Pandas, Torch, and CuDF. This project is an extension of HapSolo, which can be found here: https://github.com/esolares/HapSolo

This project is a part of an AI Research position that I've had at UC Davis since June 2022. HapSolo2 was co-developed by my lab partner, Mansi A. 

## Pandas.ipynb
The final cell in pandas.ipynb runs HapSolo2 on a specified number of cores for a set number of iterations, using Python's multiprocessing library. At completion, a specified number of solutions will be returned—with solutions being genomic assemblies with the lowest costs. To successfully execute the final cell, all cells before need to be run in order. 

## Cudf.ipynb
The second cell in Cudf.ipynb runs HapSolo2 on a specified number of cores for a set number of iterations, with Pytorch's multiprocessing package. Instead of using Pandas, this version of HapSolo2 uses cuDF. Successful execute of this notebook requires all other files in the repository to be present (except for Pandas.ipynb). Code needed to be broken up into different files for this version to address a pickling error. 


