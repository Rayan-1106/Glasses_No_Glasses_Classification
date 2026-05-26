# Glasses No Glasses Classification

## Project Overview

This project is a binary image classification system developed using deep learning. The objective is to classify face images into two categories: people wearing glasses and people not wearing glasses.

The project was implemented using Python in Google Colab. A Convolutional Neural Network model was built from scratch, and a pre-trained MobileNetV2 model was also used for comparison.

## Student Information

Student ID: 22F23625  
Student Name: Rayan Salim Rashid Al Mukhaini  
Module: Artificial Intelligence and Deep Learning  
Platform: Google Colab  

## Dataset

The dataset used in this project is the Glasses or No Glasses dataset from Kaggle.

Dataset link:  
https://www.kaggle.com/datasets/jeffheaton/glasses-or-no-glasses

The dataset contains face images and CSV files. The training CSV file includes image IDs and class labels. The labels are used to identify whether each image belongs to the Glasses or No_Glasses class.

## Tools and Libraries Used

- Python
- Google Colab
- TensorFlow
- Keras
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- PIL
- Kaggle API

## Methodology

The project follows these main steps:

1. Download the dataset from Kaggle.
2. Read the training and testing CSV files.
3. Link image IDs with the correct image files.
4. Check missing values and class distribution.
5. Display sample images with labels.
6. Split the data into training and validation sets.
7. Apply image preprocessing and data augmentation.
8. Build and train a CNN model from scratch.
9. Build and train a MobileNetV2 pre-trained model.
10. Compare both models using evaluation metrics.

## Models Used

### CNN from Scratch

A custom Convolutional Neural Network was built using Conv2D, MaxPooling2D, Flatten, Dense, and Dropout layers. Dropout was used to reduce overfitting.

### MobileNetV2

MobileNetV2 was used as a pre-trained transfer learning model. The base model was frozen, and new classification layers were added for binary classification.

## Results

| Model | Validation Loss | Validation Accuracy |
|---|---:|---:|
| CNN from Scratch | 0.2982 | 88.56% |
| MobileNetV2 | 0.2916 | 87.22% |

The CNN model achieved the highest validation accuracy and was selected as the best model for this dataset.

## Evaluation Metrics

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Conclusion

This project successfully implemented a binary image classification system for detecting whether a person is wearing glasses or not. The CNN model performed slightly better than the MobileNetV2 model, achieving approximately 88.56% validation accuracy.

Future improvements could include fine-tuning MobileNetV2, increasing the number of training epochs, applying stronger augmentation, or testing other pre-trained models such as VGG16, ResNet50, or EfficientNet.
