# Lung-Cancer-Classification-Model
This repository contains the Jupyter Notebook for a machine learning model designed to classify lung cancer using CT scan images. The model distinguishes between four types of classifications: Adenocarcinoma, Large Cell Carcinoma, Squamous Cell Carcinoma, and Normal tissue.

## Project Overview

This project demonstrates the application of deep learning techniques to medical image classification. The model is trained using a convolutional neural network (CNN) architecture with ResNet50 as the backbone, fine-tuned to identify cancerous cells from CT scan images.

Key Features:

 - Image Preprocessing: Includes data augmentation to ensure the model generalizes well across varied image orientations.
 - ResNet50 Backbone: Leveraged for its state-of-the-art performance in image classification tasks, with modifications to prevent overfitting.
 - High Accuracy: Achieved 95.6% accuracy on the test dataset, making it a robust tool for supporting radiologists in lung cancer detection.

## Data

The dataset for this project was sourced from Kaggle and includes 1,000 labeled lung CT scan images. The data was divided into:

- 70% for training
- 10% for validation
- 20% for testing

## Data Augmentation:

Data augmentation techniques such as image flipping, rotation, and zooming were applied to increase the robustness of the model.

## Model Architecture

The model utilizes the following structure:

 - ResNet50 Backbone: We use only 20 of the 50 activation layers to prevent overfitting while maintaining strong feature extraction capabilities.
 - Batch Normalization: Applied to stabilize and accelerate the training process.
 - Dropout: Added to further reduce overfitting.
 - Dense Layers: Three fully connected layers are used, with the final layer being a softmax output to predict the four classes.

The model architecture is optimized for classifying CT scan images with high accuracy and minimal loss.

## Setup Instructions

1. Clone the repository:

       git clone https://github.com/Rupert-S/Lung-Cancer-Classification-Model
    
2. Install required dependencies:

       pip install -r requirements.txt

3. Download the dataset from Kaggle and place it in the appropriate directory.
4. Run the Jupyter Notebook to preprocess the data, train the model, and generate predictions.
