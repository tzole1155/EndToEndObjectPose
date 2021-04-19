# EndToEndObjectPose
Code for our Reproducibility Challenge Paper 

## Setup
Our implementation is based on [moai](https://github.com/ai-in-motion/moai).
Please follow the intructions for installing the package.

## Data
The used dataset for running the experiments is [UAVA](https://vcl3d.github.io/UAVA/).
Please follow the instructions for downloading the data.

## Configuration files
We provide the configuration files for training the models reported in the paper. All the configuration files for conducting the reported experiments are split in unique folders containing all the necessary parts. More specifically each folder contains:
- **coordinate_regression**: Which is the main configuration file consisting of the definition of the different components.
- **data**: configuration file for creating the data loaders.
- **model**: configuration file for creating the data loaders.
- **losses**: configuration file for creating the data loaders.
- **metrics**: configuration file for creating the data loaders.
- **options**: configuration file for creating the data loaders.

## Training
To start a training, run 
```commandline
moai train --coordinate_regression.yaml <main config file> --config-dir . <path_to_configuration_files>
root=<data_path>
obj_file=<drone_obj_file>
metadata=<metadata_path>
```







