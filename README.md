# Lung Cancer Detection using Convolutional Neural Network (CNN)

## Overview
This project focuses on detecting lung cancer from histopathological images using a Convolutional Neural Network (CNN). The dataset includes 5000 images categorized into three classes: *lung_aca*, *lung_n*, and *lung_scc*. The CNN model learns intricate features from the images to classify them accurately.

---

## Dataset
The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/andrewmvd/lung-and-colon-cancer-histopathological-images). It contains 5000 histopathological images divided into three categories:
- **lung_aca**: Adenocarcinoma
- **lung_n**: Normal tissue
- **lung_scc**: Squamous cell carcinoma

The dataset is provided as a compressed file (`data.zip`) and needs to be extracted before usage.

---

## Project Workflow

### 1. Data Exploration and Visualization
- The dataset is explored and visualized to understand the image distribution across the classes.
- Random samples from each class are displayed to observe the visual patterns.

### 2. Data Preprocessing
- The images are resized to a uniform size of `256x256` pixels.
- Labels are one-hot encoded for compatibility with the CNN model.

### 3. Model Development
The CNN architecture includes:
- **Three Convolutional Layers** followed by MaxPooling Layers.
- A **Flatten Layer** to prepare the feature maps for fully connected layers.
- **Two Fully Connected Layers** to learn complex patterns in the data.
- **BatchNormalization Layers** for faster and more stable training.
- A **Dropout Layer** to prevent overfitting.
- A **Softmax Output Layer** to classify the images into three categories.

### 4. Model Training
- The model is trained for 10 epochs with early stopping based on validation accuracy.
- Hyperparameters such as learning rate, batch size, and dropout rate were optimized for better performance.

### 5. Evaluation
- The trained model achieved a training accuracy of
- Training was stopped early to prevent overfitting.
## Key Features
1. **High Accuracy**: Achieved high accuracy on both training and validation datasets.
2. **Preventing Overfitting**: Used techniques like dropout and batch normalization.
3. **Early Stopping**: Training stops automatically when validation accuracy plateaus.
