# HapSolo2

HapSolo2 is an AI optimization approach designed for the removal of secondary haplotigs in diploid genome assembly and scaffolding processes. The method employs a forward-looking randomized hill-climbing algorithm, integrating AI techniques, to minimize the cost associated with genomic assemblies. Essentially, HapSolo2 has applications to bioinformatics. 

HapSolo2 is developed completely in Python, and libraries used include Pandas, Torch, and cuDF. This project is an extension of HapSolo, which can be found here: https://github.com/esolares/HapSolo

This project is a part of an AI Research position that I've had at UC Davis since June 2022. HapSolo2 was co-developed by my lab partner, Mansi A. 
## Assembly File Placeholder
To run both the Pandas and cuDF versions of HapSolo2, please replace the placeholder assigned to myasmFileName in pandas.ipynb and start.py with the path to an assembly file in FASTA format. The assembly file I have been using is too large to upload to GitHub. 

## pandas.ipynb
The final cell in pandas.ipynb runs HapSolo2 using Python's multiprocessing library, spreading the workload across a specified number of cores for a set number of iterations. After completion, it returns a set number of solutions, which are genomic assemblies with the lowest costs. To successfully execute the final cell, all previous cells need to be executed in order.

## cudf.ipynb
In cudf.ipynb, the second cell executes HapSolo2 using a specified number of cores and PyTorch's multiprocessing package. The version of HapSolo2 executed here utilizes cuDF instead of Pandas. To address a pickling error, the code was split into separate files. Therefore, to successfully run this notebook, ensure all other repository files are present (Pandas.ipynb is not required). 


