# Melanoma Detection Assignment
* [Overview](#overview)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Contact](#contact)

## Overview  
- Out of 9 skin cancers, task is to Classify various skin cancers appropriately
- Building a model using Convolutional neural networks 
- Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert 
  dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images 
  were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose 
  images are slightly dominant. The data set contains the following diseases:

  1. Actinic keratosis
  2. Basal cell carcinoma
  3. Dermatofibroma
  4. Melanoma
  5. Nevus
  6. Pigmented benign keratosis
  7. Seborrheic keratosis
  8. Squamous cell carcinoma
  9. Vascular lesion

## Technologies Used
- TensorFlow - version 2.17.0
- Keras - version 3.4.1
- Numpy - version 1.26.4

  
## Conclusions
- First CNN model was built with 3 conv2D layers and one fully connected Dense layer
- Second CNN model built by applying some augmentation strategy to get rid of overfitting/underfitting occurred by first model and adding some Dropout layers.
- Third  model we analyzed data/sample distribution of all classes and found that there a class imbalance in dataset. By using an augmenter library, we have balanced our 
  dataset. After balancing the data, we trained our model_v3 and found that there is a significant improvement in training and validation accuracy.But the model prediction 
  is not as expected. 
- Fourth CNN model(train accuracy=88, validation accuracy=84.5) was built after applying augmentation(to overcome class imbalance in the training dataset)
- Finally choosing the best model out of three based on train and validation accuracies, Predict and evaluate Test images accuracy and loss.

## Contact
Created by [@Gadepalli Lokesh] - feel free to contact with me!

