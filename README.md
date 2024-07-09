# Cats vs. Dogs Image Classification Using SVM by Sana Liaqat

## Overview
This project classifies images of cats and dogs using a Support Vector Machine (SVM). It includes data extraction, preprocessing, feature extraction, model training, and evaluation.

## Steps

1. **Data Extraction**
   - Download and extract the "Dogs vs. Cats" dataset from Kaggle.
   - Organize the dataset into training and testing directories.

2. **Data Preprocessing**
   - Read, resize, normalize, and flatten images.

3. **Feature Extraction**
   - Apply PCA to reduce dimensionality while retaining 80% variance.

4. **Model Training**
   - Use SVM with a grid search for hyperparameter optimization.
   - Train using a pipeline with PCA and SVM.

5. **Model Evaluation**
   - Evaluate the model on the test dataset.
   - Generate accuracy, classification report, and confusion matrix.

## Usage

1. **Setup and Execution**
   - Extract the dataset.
   - Run the preprocessing script.
   - Execute the training script.
   - Evaluate the model.

2. **Output**
   - Best hyperparameters and cross-validation score.
   - Test accuracy.
   - Classification report.
   - Confusion matrix visualization.

## Results

- Best Parameters: `{'pca__n_components': 0.9, 'svm__kernel': 'rbf'}`
- Best Score: `0.6757`
- Accuracy: `0.6762`

## Files

- `confusion_matrix.png`: Confusion matrix visualization
- `classification_report.txt`: Detailed classification report
- `svm_model.pkl`: Trained SVM model

## Future Work

- Explore advanced feature extraction techniques.
- Experiment with other classifiers or ensemble methods.
- Implement data augmentation for better model robustness.

## Dataset
data: https://www.kaggle.com/c/dogs-vs-cats/data
