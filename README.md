# Spatial_Nav

## Project desc:
The aim of lab work was to study the internal representations of a deep neural network capable of rudimentary spatial navigation and tabulate the occurrences of grid-cell, object-vector-cell and other spatial cell firing fields. 

The model consisted of two pathways (LEC and MEC analogues) driven by convolved image data and path-integrated trajectories respectively. They were combined with a graph convolutional layer and processed with downstream dense layers, whose neural firing fields were examined for resemblance to spatial cells like border cells, vector cells etc. My responsibilities included debugging, maintaining the DL codebase and creating custom Unity environments.

![sn](https://github.com/erinyes-20/Spatial_Nav/assets/158277210/48f6b253-dd7e-4bd6-bf17-b6cc1d0ac3e6)

## Project workflow:
- Parsing the random trajectory generation code to create 2D paths with obstacle presence
- Creating reward sequence based on proximity to obstacle during navigation
- Obtaining image data by guiding a Unity agent through a custom environment by following 2D trajectory coordinates
- Training the neural network to output reward sequences given image data and trajectory information like head directions, orientation etc
- Tuning the hyper-parameters to vary the weightage assigned to vision-side loss vs PI loss
- Examining and iterating why said parameters were successful in evoking spatial cell representation in downstream layers

## Acknowledgements:
- Jarvez [repository](https://github.com/jarvez31/Object_representation_model)
- CNS Lab spatial nav team [publications](https://sites.google.com/view/spatialnavigators/publications)
