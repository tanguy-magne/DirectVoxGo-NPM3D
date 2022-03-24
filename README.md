# DirectVoxGo-NPM3D

Ths repository contains the work I have produced for the project of the Point Clouds and 3D Modeling course from MVA master. For this project I worked on the article *Direct Voxel Grid Optimization:Super-fast Convergence for Radiance Fields Reconstruction* [1], understanding it in details and experimenting on the different hyperparameters.

To run the code, simply open the notebook `colab_DirectVoxGO.ipynb` on colab.

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

## Results

Here are some results obtained.

### Robot scene from NSVF-Synthetic dataset

https://user-images.githubusercontent.com/91187810/159984751-1f97c950-5a9c-4784-8cd0-c463ded0034c.mp4

Left : Ground Truth | Middle : Results using pre-activation | Right : Results using post-activation

### Custom forward facing scene

https://user-images.githubusercontent.com/91187810/159985003-d9d85f49-e5b4-46da-9ae1-ae3a7708a717.mp4

Here the results seems really good.

https://user-images.githubusercontent.com/91187810/159985017-5be21c6d-5823-4568-a402-c8ce5b5faeaa.mp4

However here, the results are not so good, because the range of viewpoints is too important.


## References

[1] Cheng Sun, Min Sun, and Hwann-Tzong Chen. Direct voxel grid optimization: Super-fast convergence for radiance fields reconstruction. *arXiv preprint arXiv:2111.11215*, 2021.
