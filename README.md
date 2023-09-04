# Data Science Lab Computer Vision course with Python
## 2. Deep Learning with PyTorch

This course is an introduction to Deep Learning for Computer Vision using PyTorch. It is part of the [Data Science Lab](https://www.dsl.unibe.ch/) course on Computer Vision with Python. The goal of the course is to give an overview over how PyTorch functions, how to feed image data to models etc. and is not meant as a theoretical course on Deep Learning or or to provide details on efficiently training models. There are roughly three parts:
- introduction to tensors and anatomy of a neural network
- feeding images to models and basics of training
- using pre-trained models

## Getting the material

To use all notebooks locally, you can simply clone (if you know git) or download the repository by using the green "Code" button at the top right of the repository. Place the folder in easily reachable location on your computer.

You can download all necessary data from [this link](). Place the main data folder then in the main folder of the downloaded repository for paths to be correct.

## Setting up an environment

A series of packages is necessary to run the content of this notebook. We highly recommend to install packages within an environment such as provided by conda. There are multiple ways to install conda and if you don't yet have a version installed we strongly recommend to use mambaforge which will install the fast environment solver mamba. You can find installers at [this link](https://github.com/conda-forge/miniforge#mambaforge). 

Note that you can use mamba also from an older conda installation. For this follow these steps (described [here](https://www.anaconda.com/blog/a-faster-conda-for-a-growing-community):
1. Update conda:
    ```conda update -n base conda```
2. Install mamba:
    ```conda install -n base conda-libmamba-solver```
3. Use mamba as a solver:
    ```conda config --set solver libmamba```

Once you have conda/mamba installed, open a terminal where you have access to conda (i.e. the beginning of the line on your terminal window should indicate ```(base)```). On MacOS or Linux, your regular terminal should work. On Windows, depending how you installed conda, you might only have access to it from a terminal called XXX Prompt where XXX stands for Anaconda, Miniforge etc. depending how conda was installed.

Then in that terminal head to the folder of the repository you downloaded previously. In the main folder you will find an [environment.yml](environment.yml) file that contains infos about all packages to install. You can simply create the necessary environment using:

    mamba env create -f environment.yml

if you have mamba installed or

    conda env create -f environment.yml

This creates an environment called ```dslpytorch``` that you then need to activate (here mamba or conda doesn't matter):

    conda activate dslpytorch

Finally you can start Jupyterlab using:

    jupyter lab

This should automatically open a Jupyterlab session in your favorite browser. If not, copy the address appearing in the terminal starting with ```http://localhost:8888...``` in your browser.

## Google Colab

If installation fails or isn't working properly, a fallback solution is to use Google's version of Jupyter called Colab. You can open the notebooks of this course using this button: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/guiwitz/DSL_CV1_numpy_skimage/blob/colab). Most packages come pre-installed and missing ones can be installed "on the fly" in each notebook.

## Authors

Guillaume Witz, Data Science Lab, University of Bern