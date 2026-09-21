# A Computer Vision Approach for Automated Identification of Cassava Diseases

This project focuses on using computer vision and deep learning to automatically identify cassava diseases from leaf images. The goal is to support early detection and diagnosis, helping farmers and agricultural professionals act quickly to reduce crop loss.

<img width="908" alt="image" src="https://github.com/user-attachments/assets/3e6e7603-8331-4d7a-8fb1-426ccb104454">

## Project Overview

A machine learning model was trained to detect and classify cassava diseases using image data. The system successfully identifies the following conditions:

- Cassava mosaic disease (CMD)
- Cassava bacterial blight (CBB)
- Cassava brown streak disease (CBSD)

These diseases can severely affect cassava production, and early automated detection can help prevent further spread and improve crop management.

## Why This Matters

Cassava is a major staple crop in many African countries, and disease outbreaks can have a significant impact on food security and farmer livelihoods. Rapid disease recognition is crucial because some infected plants must be removed or managed quickly to prevent transmission.

This project applies deep learning techniques to analyze leaf images and distinguish between disease patterns with a high level of accuracy.

## Dataset

The model was trained on a cassava leaf disease dataset containing labeled images of healthy and diseased leaves. The dataset includes image files for the training and testing process, with disease labels mapped to their real names.

### Data Attributes

- image_id - image file name
- label - ID code for the disease
- label_num_to_disease_map.json - mapping between each disease code and the real disease name

<img width="1023" alt="image" src="https://github.com/user-attachments/assets/c8c52873-60c0-441c-97c5-fabfad1c6142">
<img width="996" alt="image" src="https://github.com/user-attachments/assets/ae820d13-6a0d-492c-86a0-442ef9b45cdc">


**Environment:** Kaggle

## Model and Tools

This project uses PyTorch for model development and training, along with standard data science libraries for preprocessing, analysis, and visualization.

### Libraries
- PyTorch
- pandas
- scikit-learn
- numpy
- matplotlib
- seaborn

### Neural Network

- ResNet-152 architecture

**Accuracy:** 89%

## Summary

This repository demonstrates a practical computer vision approach for automated cassava disease identification. By training a deep learning model on leaf images, the project aims to support faster, more reliable diagnosis of cassava diseases in agricultural settings.
