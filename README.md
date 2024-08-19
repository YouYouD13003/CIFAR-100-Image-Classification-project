# CIFAR-100-Image-Classification-project

# I.A/python Project - CIFAR-100 Image Classification

**Author:** ABBES Ayoub

## Project Overview

This project implements a Convolutional Neural Network (CNN) to classify images from the CIFAR-100 dataset, which contains 60,000 32x32 color images across 100 classes. The model was designed to effectively learn and generalize patterns within the dataset, achieving a test accuracy of 72.74%.

## Key Features

- **Data Preprocessing:** 
  - Normalized pixel values to [0, 1].
  - One-hot encoding of labels for 100 classes.

- **Model Architecture:** 
  - Multiple convolutional blocks with Batch Normalization, ReLU activation, MaxPooling, and Dropout layers.
  - Flattening followed by a Dense layer with 512 units and an output Dense layer with 100 units using softmax activation.

- **Training Strategy:**
  - Optimized using the Adam optimizer with categorical cross-entropy loss.
  - Initial learning rate set to 0.0005 with a custom learning rate scheduler.
  - Data augmentation techniques such as rotation, shift, zoom, and horizontal flip were applied in real-time.
  - Employed callbacks like EarlyStopping, ModelCheckpoint, LearningRateScheduler, and ReduceLROnPlateau to fine-tune the training process.

## Results

- **Performance:** The model achieved a test accuracy of 72.74% and a test loss of 1.0696.
- **Confusion Matrix Analysis:** Demonstrates good classification performance with minor misclassifications, typical given the complexity of CIFAR-100.

## Conclusion

This project successfully developed a CNN capable of classifying CIFAR-100 images with a high degree of accuracy. Future improvements could include exploring more advanced data augmentation, deeper architectures, or alternative regularization techniques to further boost performance.
