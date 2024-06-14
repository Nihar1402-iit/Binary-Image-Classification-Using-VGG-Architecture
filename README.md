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

## Models Implemented

### VGG-Model (1 Block)
- Implemented using PyTorch with a single convolutional block.
- Trained and evaluated on a custom animal image dataset.

### VGG-Model (3 Blocks)
- Custom VGG-like architecture with three convolutional blocks.
- Utilizes data augmentation techniques for improved model robustness.

### VGG16-Model (Transfer Learning)
- **VGG16_tl**: Transfer learning with fine-tuning only the final MLP layers.
- **VGG16_tl_all**: Transfer learning with fine-tuning all layers of VGG16.

## Tensorboard Integration

### Functionality
- **log_images**: Logs images and their predictions on the test dataset to Tensorboard.
- **Confusion Matrix**: Visualizes the confusion matrix for model predictions on the test dataset.

### Implementation Steps
1. Imports necessary libraries including TensorFlow, PyTorch, and others.
2. Defines model architectures (VGG1Block, VGG3Block, VGG16_tl, VGG16_tl_all) and loads trained model weights.
3. Loads test data using PyTorch DataLoader and transforms.
4. Utilizes TensorFlow's `tf.summary` to log images and confusion matrices to Tensorboard.
5. Evaluates each model on the test dataset and calculates accuracy metrics.
6. Cleans up existing logs directory and creates new logs for each model.

### Usage
- Each model's evaluation results, including accuracy and confusion matrix, are logged to a separate directory under `logs/`.
- Tensorboard can be launched to visualize these metrics by running `%tensorboard` after executing the notebook or script.

For detailed evaluation and visualization of model performance using Tensorboard, refer to the generated logs. Adjust paths and configurations as needed based on your specific setup.

## Tensorboard Link
[View Tensorboard Logs](logs/)
### VGG16 Architecture
- **VGG16**: Pre-trained VGG16 model for image classification tasks.

## Evaluation and Metrics
- Each model is trained and evaluated on a custom animal image dataset.
- Performance metrics such as training time, training loss, training accuracy, and testing accuracy are reported for each model.
- Data augmentation techniques are applied to enhance model generalization and robustness.

## Subjective Analysis
- Answering subjective questions related to model performance, the impact of data augmentation, optimal number of training epochs, and specific image cases where models exhibit confusion.

