# Skin_Disease_Classifier-using-ML
This Model is built using Google Colaboratory in the beginning to benefit the Virtual GPU and optimize development of the model. 
This document contains entire understanding of the model.
Model is built using Google Colaboratory in the beginning to benefit the Virtual GPU and optimize development of the model.
## Introduction
### Significance: 
The proposed project holds immense significance due to its potential to address
several critical issues in the field of skin disease diagnosis:
### Early Detection:
Machine learning algorithms can analyze skin images to detect subtle
changes that might not be easily noticeable to the naked eye. Early detection is crucial for
improving treatment outcomes and reducing the progression of diseases.
### Access to Healthcare: 
Especially in remote or underserved areas, individuals often lack access
to dermatologists. A ML-powered system can act as a preliminary screening tool, offering
timely guidance on whether a professional consultation is necessary.
### Reducing Misdiagnosis: 
Skin diseases often share visual similarities, leading to misdiagnosis.
ML algorithms, trained on large datasets, can learn to differentiate between these conditions
with a high degree of reducing errors.

## Project Overview:
We have used several layers in the model which provide Block-wise approach to detect and classify skin diseases. 
This contains several layers such as MaxPooling2D, Conv2D, Dense, Dropout, Flatten, and Batch Normalization.
We have used two datasets and combined them after cleaning, annotating, and preprocessing of the dataset to obtain better results.
The first dataset is DermNet, which required cleaning, and annotating the dataset.
The second dataset is ISIC 2019, which also required to be cleaned and annotating.
This model works on FIVE types of Skin Disease Detection
Using analysis we have chosen the most common types of skin diseases in the region.
This model took us almost an year to be built with multiple collaborators in order to acheive a validation accuracy of 90%.
This model was tested on InceptionV3 and VDD based models which did not perform any better, infact it performed worse.
This has a custom CNN based model which has Block-wise approach through layers to detect and identify skin disease from an image.

The steps required for anyone to run this model can be acheived by downloading the dataset and the model files.
Which soon will be updated by time in order for everyone to use it.
## Data Collection & Preprocessing:
We have used two datasets and combined them and used FIVE Skin Diseases.
Using analysis we have chosen the most common types of skin diseases in the region, that are:
### DermNet (Kaggle)
### ISIC 2019 (IEEE)
These datasets were unclean and the performance of the model on this dataset were poor.
We manually cleaned both datasets for unclear images.
We chose to keep the number of images close between diseases.
### Duplicate Image Removal:
Identify and remove duplicate images from the dataset to ensure that each image is unique.
Duplicate images can skew the training process.
### Metadata Validation:
Validate and clean the metadata associated with the images. Ensure that patient information is
appropriately anonymized, and any confidential data is removed or obscured.
Handling Missing Data:
Address missing data issues by identifying images with incomplete metadata or corrupted files.
24
For missing metadata, if possible, retrieve or complete the necessary information from reliable
sources.
For missing or corrupted images, consider image reconstruction techniques or remove the
affected samples.
### Data Standardization:
Standardize image resolution to a common size to ensure uniformity in the dataset. Resizing
images to a consistent resolution (e.g., 124x124 pixels) is often necessary for model
compatibility.
### Color Normalization:
Normalize the colors of the images to mitigate variations caused by lighting conditions, camera
settings, and other factors. Techniques like histogram equalization or color channel
normalization can be applied.

## Model Building:
This model took us almost an year to be built with multiple collaborators in order to acheive a validation accuracy of 90%.
This model was tested on InceptionV3 and VDD based models which did not perform any better, infact it performed worse.
This has a custom CNN based model which has Block-wise approach through layers to detect and identify skin disease from an image.
### Libraries and Frameworks:>
#### Numpy
#### openCV
#### TensorFlow
#### Keras
#### Matplotlib
#### Seaborn
### IDE:
#### Google Colab
#### Jupyter Notebook

## Results
### Epochs.
<img width="778" alt="1 to 5 epochs" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/61749e40-1c9a-478e-8598-30513c890e55">
<img width="702" alt="95 to 100 epochs" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/ec68d556-9a05-418f-9632-9ffab50a7630">
### Accuracy and Loss Plotting:
<img width="457" alt="Model Accuracy" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/971e0af4-66ca-4613-b903-5f747e4f90eb">
<img width="427" alt="Model Loss" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/be399ede-6315-4bbd-b12d-7b1911fab8c3">
### Color Bar/ Confusion Matrix:
<img width="346" alt="Confusion Metrix" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/6138cf7b-0184-443a-9956-2a63199ad353">
### HeatMap
<img width="367" alt="Heat Map" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/7331637f-e177-43e3-b3ed-2f1e57f4d3d3">
### Results compared with different Architectures:
<img width="509" alt="Table" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/81ad6184-3fb1-4e86-ad97-df44527972f9">

## Deployment:
We have currently used Streamlit to execute the model for now.

## Real Time Testing:
<img width="284" alt="pre 1" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/f8b23fc2-b73f-4099-93df-91a3b46c8001">
<img width="287" alt="pre 2" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/a3198f4f-f405-4004-bffa-ff12058ff505">
<img width="284" alt="pre 3" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/c7d1f9d7-00c9-41cc-a8fc-227c664a189c">
<img width="285" alt="pre 4" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/8f59f919-fc55-4263-aa63-a6c80a58d240">
<img width="298" alt="Acne 5" src="https://github.com/Muzamil02/Skin_Disease_Classifier-using-ML/assets/96439773/20e50047-ea53-43eb-8fe1-eb647d7ba1cb">
