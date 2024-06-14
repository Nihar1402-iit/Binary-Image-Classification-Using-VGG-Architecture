# Binary-Image-Classification-Using-VGG-Architecture

This repository contains implementations of various convolutional neural network (CNN) models for animal classification tasks using PyTorch and TensorFlow/Keras. The models and techniques included are:

## PyTorch Models

### Custom VGG-like Architectures
- **VGG1Block**: A custom VGG-like architecture with a single convolutional block.
- **VGG3Block**: A custom VGG-like architecture with three convolutional blocks.
- **VGG3Block with Data Augmentation**: VGG3Block architecture integrated with data augmentation techniques to improve model robustness.

### Transfer Learning with VGG16
- **VGG16_tl**: Transfer learning using VGG16 with fine-tuning only the final MLP layers.
- **VGG16_tl_all**: Transfer learning using VGG16 with fine-tuning all layers.

### Multi-Layer Perceptron (MLP) Model
- **MLP Model**: An MLP model designed for image classification, with customizable layer configurations. It is evaluated alongside CNN models like VGG1Block, VGG3Block, and VGG16 variants.

## TensorFlow/Keras Models

### VGG16 Architecture
- **VGG16**: Pre-trained VGG16 model for image classification tasks.

## Evaluation and Metrics
- Each model is trained and evaluated on a custom animal image dataset.
- Performance metrics such as training time, training loss, training accuracy, and testing accuracy are reported for each model.
- Data augmentation techniques are applied to enhance model generalization and robustness.

## Subjective Analysis
- Answering subjective questions related to model performance, the impact of data augmentation, optimal number of training epochs, and specific image cases where models exhibit confusion.

