# Melanoma-Detection

> To develop a CNN-based model capable of accurately detecting melanoma, a potentially fatal form of cancer if not identified early. Melanoma is responsible for 75% of skin cancer-related deaths. An AI-driven solution that analyzes images and alerts dermatologists to its presence can significantly reduce the manual effort required for diagnosis, enabling faster and more efficient detection.
 
## Table of Contents
* [Problem Statement](#problem-statement)
* [Project Pipeline](#project-pipeline)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Problem Statement

### Business Understanding

The dataset comprises 2,357 images of malignant and benign oncological diseases, sourced from the International Skin Imaging Collaboration (ISIC). The images are categorized based on ISIC classifications, ensuring balanced subsets, except for melanomas and moles, which have a slightly higher representation.


The data set contains the following diseases:

* Actinic keratosis
* Basal cell carcinoma
* Dermatofibroma
* Melanoma
* Nevus
* Pigmented benign keratosis
* Seborrheic keratosis
* Squamous cell carcinoma
* Vascular lesion

### Business Goal:

Build a multiclass classification model using a custom convolutional neural network in TensorFlow. 

### Business Risk:

- Predicting a incorrect class of skin cancer

## Project Pipeline
- Data Reading/Data Understanding → Defining the path for train and test images 
- Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
- Model Building & training : 
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit.
- Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
- Model Building & training on the augmented data :
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~20 epochs
  - Write your findings after the model fit, see if the earlier issue is resolved or not?
- Class distribution: Examine the current class distribution in the training dataset 
  - Which class has the least number of samples?
  - Which classes dominate the data in terms of the proportionate number of samples?
- Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.
- Model Building & training on the rectified class imbalance data :
  - Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
  - Choose an appropriate optimiser and loss function for model training
  - Train the model for ~50 epochs

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Technologies Used
- TensorFlow version: 2.18.0
- Keras version: 3.9.0
- Matplotlib version: 3.10.0
- NumPy version: 1.26.4
- Pandas version: 2.2.2
- PIL version: 10.3.0
- Augmentor version: 0.2.12


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Author [@sudhindrasaxena] 
