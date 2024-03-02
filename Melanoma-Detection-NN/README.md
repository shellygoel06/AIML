## Multiclass Classification Model Using a Custom Convolutional Neural Network
>To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Problem Statement
Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths.

## Objective of the Project

- To build a CNN based model which can accurately detect melanoma. 
- To build a multiclass classification model using a custom convolutional neural network in TensorFlow.
- A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
1. Introduction 
    - Problem Statement
    - Objective of the Project
2. Importing all the Required Libraries
3. Data Reading/Data Understanding
    - Defining the path for train and test images
4. Dataset Creation
    - Creating Batch Size
    - Resizing Images
    - Create, train & validation dataset from the train directory
5. Dataset Visualisation
    - Visualize all the Classes Present in the Dataset 
6. Model Building & training
    - Create the Model
    - Compile the Model
    - Train the Model
    - Visualizing the Model
    - Findings of the Model
7. Model Building & training on the augmented data
    - Create the Model
    - Compiling the Model
    - Training the Model
    - Visualizing the Results
8. Class distribution
9. Handling class imbalances
    - Train the model on the data createdusing Augmentor
    - Create a training dataset
    - Create a validation dataset
    - Create your model(make sure to include normalization)
    - Compile your Model(Choose Optimizer and Loss Function)
10. Model Building & training on the rectified class imbalance data
    - Train your Model
    - Visualize the Model Results
    - Findings

The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.


## The data set contains the following diseases:

1. Actinic keratosis
2. Basal cell carcinoma
3. Dermatofibroma
4. Melanoma
5. Nevus
6. Pigmented benign keratosis
7. Seborrheic keratosis
8. Squamous cell carcinoma
9. Vascular lesion

* [Technologies Used]

- Python
- Tensorflow

* [Conclusions]

- The class rebalance helped in reducing overfititng of the data and thus the loass is beng reduced But it reduced the Acurracy very low
- Then we introduced dropout which reduced the over fit
- At last we tried Batch Normalization and Augumentation which really helped in carry forward
- We can also see that validation accuracy is also around 84%, which is very close to training accuracy, hence there is no overfitting/underfitting
- The model was also evaluated with more data augmentation techniques but the accuracy reduced a lot because of varying differences between images. But it can be rectified by training it for more number of epochs.

* [Acknowledgements](#acknowledgements)


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by - Upgrad
- References if any...
- This project was based on Upgrad Learning


## Contact
Created by [@shellygoel06] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
