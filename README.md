# Fine-tuning VGG16 for Cat and Dog Classification

## Description:
This repository contains Python code for fine-tuning the VGG16 convolutional neural network architecture to classify images of cats and dogs. The code is implemented using the Keras deep learning framework.

## Dataset
https://www.kaggle.com/datasets/arnaudeq/cats-vs-dogs-1000

## Explanation:
The code follows these main steps:
1. **Loading Pre-trained VGG16 Model**: The pre-trained VGG16 model is loaded from Keras with ImageNet weights.
2. **Customizing the Model**: The fully connected layers are replaced with custom dense layers for fine-tuning.
3. **Freezing Layers**: All layers except custom dense layers are frozen to retain pre-trained weights.
4. **Compiling the Model**: Model is compiled with categorical cross-entropy loss and Adam optimizer.
5. **Data Preparation**: ImageDataGenerator preprocesses and augments training and validation data.
6. **Training the Model**: Custom VGG16 model is trained with augmented data.
7. **Saving the Model**: Trained model is saved in HDF5 format.
8. **Loading Saved Model**: Saved model is loaded for inference on new images.
9. **Prediction**: Model predicts class labels of test images (cats or dogs).

This code demonstrates transfer learning for image classification tasks, offering insights into fine-tuning pre-trained models for specific domains.

## How to Use:
1. Clone this repository to your local machine.
2. Ensure you have Python installed, along with the necessary libraries specified in `requirements.txt`.
3. Run the Jupyter notebook `cat_dog_vgg16_2.ipynb` to execute the code step-by-step.
4. Follow the instructions within the notebook to customize, train, and save the model.
5. For prediction on new images, load the saved model and use the provided code snippets to predict class labels.

Feel free to adjust and expand upon the code and instructions as needed!
