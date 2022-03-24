# DirectVoxGo-NPM3D

Ths repository contains the work I have produced for the project of the Point Clouds and 3D Modeling course from MVA master. For this project I worked on the article *Direct Voxel Grid Optimization:Super-fast Convergence for Radiance Fields Reconstruction* [1], understanding it in details and experimenting on the different hyperparameters.

## Structure of the repository

This repository is an extension of the original article repository. It contains the repository with some modification in the folder DirectVoxGO. The structure of the FirectVoxGO folder is the following :

    data
    ├── configs # folder containing all configs for al models
    │
    ├── figs # folder containing figures of the original repository
    │
    ├── lib # folder containing the main models (dvgo and dmipgo) and the data loader for l datasets
    │
    ├── llff # folder scripts to convert output from COLMAP into input of the model, taken om https://github.com/Fyusion/LLFF
    │
    └── tools # visualization tools from the original repo 

In addition to this folder, this repository contains a notebook `colab_DirectVoxGO.ipynb` that allows to run experiments on colab.

## References

[1] Cheng Sun, Min Sun, and Hwann-Tzong Chen. Direct voxel grid optimization: Super-fast convergence for radiance fields reconstruction. *arXiv preprint arXiv:2111.11215*, 2021.
