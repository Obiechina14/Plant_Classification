# Plant Disease Classification

This project aims to classify plant diseases using a Convolutional Neural Network (CNN) with the MobileNetV2 architecture. The model is trained on an augmented dataset of plant disease images and deployed as a web application using Flask.

## Table of Contents
- Overview
- Dataset
- Model Architecture
- Training
- Deployment
- Usage
- Contributing


## Overview
Plant diseases can significantly impact agricultural productivity. This project provides a solution to classify plant diseases from images using deep learning techniques.

## Dataset
The dataset used in this project is the Kaggle "New Plant Diseases Dataset (Augmented)" which contains about 87000 images of various 38 plant diseas classes. The dataset is split into training, validation, and test sets.

## Model Architecture
The model is built using the MobileNetV2 architecture, pre-trained on ImageNet. The top layer is removed, and custom layers are added for the classification task.

## Training
The model is trained using the following steps:
1. **Data Augmentation**: Applied transformations like rescaling, shearing, zooming, and horizontal flipping.
2. **Model Compilation**: Compiled with Adam optimizer and categorical cross-entropy loss.
3. **Callbacks**: Used early stopping and model checkpointing to save the best model.
4. **Training**: Trained for 20 epochs with a batch size of 128.

## Deployment
The trained model is deployed as a web application using Flask. The app allows users to upload images and get predictions on the plant disease.

### Running the Flask App Locally
1. Install the required packages:
   ```bash
   pip install Flask tensorflow
Run the Flask app:
flask run --host=0.0.0.0

## Usage
Web Application: Upload an image of a plant leaf to the web app to get the disease classification.

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
