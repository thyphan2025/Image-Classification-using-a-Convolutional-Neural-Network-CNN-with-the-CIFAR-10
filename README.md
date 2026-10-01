# Image Classification using a Convolutional Neural Network CNN with the CIFAR-10

This notebook demonstrates a complete workflow for image classification using a Convolutional Neural Network (CNN) with the CIFAR-10 dataset in TensorFlow/Keras.

## Key steps include:

**1. Data Loading and Preparation:**
The CIFAR-10 dataset (60,000 color images, 10 classes) is loaded, and pixel values are normalized to a 0-1 range. A visualization of the first 25 training images is provided to verify the dataset.

**2. CNN Model Definition:**
A sequential Keras model is constructed, featuring a convolutional base with Conv2D and MaxPooling2D layers, followed by Flatten and Dense layers for classification. The architecture includes three convolutional blocks, increasing filters from 32 to 64. The model summaries at different stages illustrate the tensor shape transformations.

**3. Model Compilation and Training:**
The model is compiled using the adam optimizer and SparseCategoricalCrossentropy loss function. It's then trained for 10 epochs with a batch size of 160, with validation on the test set.

**4. Model Evaluation:**
After training, the model's performance is evaluated on the test dataset, and the test accuracy is printed. A plot showing the training and validation accuracy over epochs is generated to visualize learning progress.
