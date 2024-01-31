# SMOKE-detection-using-DNN

## Overview

This repository contains the necessary files and instructions for deploying a smoke detection model based on the VGG16 architecture. The model has been trained on a dataset of 6000 images in TIFF format.

## Model Architecture

The VGG16 model achieved an accuracy of 86.27%, outperforming the ResNet50V2 model (84.34%) in terms of accuracy.

### VGG Architecture:

1. Background:

Developed by the Visual Geometry Group at the University of Oxford.
Proposed in the paper titled "Very Deep Convolutional Networks for Large-Scale Image Recognition" in 2014.

2. Architecture:

VGG is known for its simplicity and uniformity in architecture.
It consists of 16 convolutional layers or 19 layers, depending on the specific variant (VGG16 or VGG19).
Uses small 3x3 convolutional filters throughout the network with max-pooling layers in between.

3. Characteristics:

VGG has a homogeneous architecture with small receptive fields, making it easy to understand and implement.
It achieved good performance on image classification tasks and was one of the first deep convolutional neural networks to gain popularity.


### ResNet50 Architecture:

1. Background:

ResNet (Residual Network) was introduced in the paper "Deep Residual Learning for Image Recognition" by Microsoft Research in 2015.
The "50" in ResNet50 indicates the number of layers.

2. Architecture:

ResNet introduces the concept of residual learning, where the network learns residual functions instead of directly learning the desired mappings.
ResNet50 consists of 50 layers, with a unique residual block design.
It uses skip connections (shortcuts) to skip one or more layers, allowing the model to learn residuals with respect to the layer inputs.

3. Characteristics:

ResNet addresses the vanishing gradient problem by introducing residual connections, enabling the training of very deep networks.
Residual blocks help in training deeper networks without suffering from degradation issues.


### Comparison:

1. Depth:

VGG has a relatively straightforward architecture with a fixed depth of either 16 or 19 layers.
ResNet50, on the other hand, is deeper, with 50 layers, thanks to the use of residual blocks.

2. Parameter Efficiency:

ResNet is known for being more parameter-efficient and easier to train on very deep architectures due to the residual connections.
VGG, while effective, can be computationally expensive and requires more parameters.

3. Performance:

In general, both VGG and ResNet are powerful architectures, but ResNet50 often outperforms VGG on large-scale image recognition tasks, especially as the depth of the network increases.


4. Ease of Interpretability:

VGG is more interpretable due to its simple and uniform structure.
ResNet, with its residual connections, might be a bit more complex to interpret, but it has shown superior performance in practice.
Both the models have been tried in this project


## Dataset

The dataset used for training and testing consists of 6000 images in TIFF format. Ensure that the dataset is organized with appropriate folders for training and testing, following the directory structure:


![image](https://github.com/praveen-raj-m/smoke-detection-using-DNN/assets/75660847/47e521bc-7fda-48db-bfd4-11d9dc9f2a5d)

![image](https://github.com/praveen-raj-m/smoke-detection-using-DNN/assets/75660847/86eef705-12a8-4cb4-b4b2-d79e4b65d557)

![image](https://github.com/praveen-raj-m/smoke-detection-using-DNN/assets/75660847/457858fc-6a40-42b3-8f31-0edeca882302)


## Conclusion

In the comparison between VGG16 and ResNet50V2 for smoke detection, the VGG16 architecture demonstrated superior accuracy with a value of 86.27%, outperforming ResNet50V2, which achieved an accuracy of 84.34%. The simplicity and homogeneity of VGG16, coupled with its competitive performance, make it a suitable choice for the smoke detection task. The provided deployment instructions guide users through cloning the repository, installing dependencies, and seamlessly integrating the pre-trained VGG16 model into their applications or systems. 
