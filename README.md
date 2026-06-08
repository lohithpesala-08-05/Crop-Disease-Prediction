# Crop Disease Prediction using CNN

## Project Overview

This project uses a Convolutional Neural Network (CNN) to identify crop diseases from leaf images. The model is trained on the PlantVillage dataset and can classify images into 38 different disease and healthy crop categories.

## Dataset

The dataset used in this project is the PlantVillage dataset.

Dataset Link:
https://www.kaggle.com/datasets/emmarex/plantdisease

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Matplotlib
* Scikit-learn

## Model Architecture

The CNN model consists of:

* Convolutional Layers
* Max Pooling Layers
* Global Average Pooling Layer
* Dense Layers
* Dropout Layer

Image Size: 224 × 224

Number of Classes: 38

## Project Results

* Validation Accuracy: 91.06%
* Validation Loss: 0.2815
* Weighted Precision: 91%
* Weighted Recall: 91%
* Weighted F1-Score: 91%

## Manual Testing

| Actual Class             | Predicted Class          | Confidence | Result    |
| ------------------------ | ------------------------ | ---------- | --------- |
| Apple___Apple_scab       | Apple___Apple_scab       | 69.98%     | Correct   |
| Tomato___Early_blight    | Tomato___Early_blight    | 52.81%     | Correct   |
| Soybean___healthy        | Soybean___healthy        | 99.99%     | Correct   |
| Strawberry___Leaf_scorch | Strawberry___Leaf_scorch | 99.95%     | Correct   |
| Grape___Black_rot        | Grape___Black_rot        | 95.99%     | Correct   |
| Potato___healthy         | Soybean___healthy        | 49.75%     | Incorrect |

## Features

* Crop disease classification using CNN
* Data augmentation for better generalization
* Confusion matrix and classification report
* Disease prediction on custom leaf images
* Model saving and loading using Keras

## Limitations

* Model performs best on PlantVillage-style images.
* Performance may decrease on real-world field images with complex backgrounds.
* Some classes such as Potato Healthy show lower recall.

## Future Enhancements

* Transfer Learning using MobileNetV2 or EfficientNet
* Web deployment using Streamlit
* Real-time disease detection
* Training on more real-world farm images


