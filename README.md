# DPG Workflows tutorial 2023

Repository link: https://github.com/pyiron/dpg-workflows-tutorial-2023

This repository contains the materials presented during the DPG workflows tutorial organised on 26 March 2023. 

## Creating the environment

The conda environment which includes all the necessary packages is specified in the `environment.yml` file. The environment can be created using:

```
conda env create -f environment.yml  
```

Once the environment is created, it can be activated using `conda activate potentials`. Additionally the following commands need to be run to install other necessary packages.

```
git clone https://github.com/ICAMS/TensorPotential
cd TensorPotential
python setup.py install
cd ..

git clone https://github.com/ICAMS/python-ace
cd python-ace
python setup.py install
cd ..
```

## Building the documentation

To be build the documentation, from the main directory, run:

```
jb build .
```

You can view the documentation at [`_build/index.html`](_build/index.html).
