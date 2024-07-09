# Cats vs. Dogs Image Classification Using SVM by Sana Liaqat

## Overview
This project focuses on developing an image classification system to distinguish between images of cats and dogs using machine learning techniques. The dataset employed is the "Cats vs Dogs" dataset, which contains a collection of labeled images of cats and dogs. The goal is to train a model that can accurately classify new images as either a cat or a dog.

## Key Components and Techniques:

1. Data Acquisition and Preprocessing:

The project begins with acquiring the "Cats vs Dogs" dataset, which is then split into training and validation sets. The images undergo preprocessing, including resizing and normalization, to standardize them for model training.

2. Data Augmentation:

To enhance the diversity and quantity of training data, image augmentation techniques are applied using TensorFlow's ImageDataGenerator. These techniques include rotation, width and height shifting, shearing, zooming, and horizontal flipping. Augmented images help in improving the model's ability to generalize from the training data.

3. Model Training - Convolutional Neural Network (CNN):

Initially, a CNN model is trained on the augmented training data. The CNN consists of multiple convolutional and pooling layers followed by fully connected layers. It learns hierarchical representations of the input images, capturing features that distinguish between cats and dogs.

4. Feature Extraction and SVM Training:

Features extracted from the trained CNN model are used as input to an SVM classifier. These features represent high-level characteristics of the images that are crucial for classification. The SVM model, trained using these features, learns to delineate between cats and dogs based on the extracted feature representations.

5. Model Evaluation:

The performance of the SVM model is evaluated using the validation dataset. Metrics such as accuracy are computed to assess how well the model generalizes to unseen data. This evaluation ensures that the model can reliably classify new images of cats and dogs.
Prediction:

Once trained and validated, the SVM model is capable of predicting the class (cat or dog) of new images provided by the user. The model's predictions are displayed alongside the input images, demonstrating its classification capabilities.

6. Conclusion:

This project illustrates the process of building an image classification system using both deep learning (CNN) and traditional machine learning (SVM) techniques. It highlights the importance of data augmentation, feature extraction, and model evaluation in developing robust and accurate image classifiers.

## Dataset
data: https://www.kaggle.com/c/dogs-vs-cats/data
