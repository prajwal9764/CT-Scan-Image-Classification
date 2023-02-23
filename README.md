# CT-Scan-Image-Classification
CT Scan Classification using ResNet50
This repository contains code for classifying CT scans using ResNet50, a deep learning model trained on the Image dataset. The goal of this project is to accurately classify CT scans as either COVID Positive or Negative.

# Dataset
The dataset used for this project is the CT Scan Images dataset, which consists of 1,252 COVID and 1,229 NON-COVID CT scans in png format.

# Model
The ResNet50 model is used for classification. The pre-trained weights are loaded and the last layer is replaced with a new layer for binary classification. The model is trained on the training set for 10 epochs, using binary cross-entropy loss and Adam optimizer.

Performed data augmentation on the images using the ImageDataGenerator class from
the Keras library. I used five arguments for data augmentation, namely, rotation range, width
shift range, height shift range, shear range, and zoom range. Data augmentation is a technique
used to create new training examples by augmenting the existing data with modified versions of
images. This helps to prevent overfitting of the model by providing a more diverse training set

The model achieves an accuracy of 59% on the validation set. The precision, recall, and f1-score are included in the results directory.
