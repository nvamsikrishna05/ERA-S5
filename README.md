# Handwritten Digits Classification using Convolution Neural Network (CNN)

This repo contains code for building a CNN model which is trained on the MNIST dataset for Handwritten Digits Classification

## File Structure

`model.py` contains the CNN Model. Summary of the Model - 
```
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 32, 26, 26]             320
            Conv2d-2           [-1, 64, 24, 24]          18,496
            Conv2d-3          [-1, 128, 10, 10]          73,856
            Conv2d-4            [-1, 256, 8, 8]         295,168
            Linear-5                   [-1, 50]         204,850
            Linear-6                   [-1, 10]             510
================================================================
Total params: 593,200
Trainable params: 593,200
Non-trainable params: 0
----------------------------------------------------------------
```

`utils.py` contains the utility functions for training the model, testing the model, plotting the training metrics of the model

`S5.ipynb` contains the code for Using the MNIST Dataset and training the model

## How to Use

Open the `S5.ipynb` file and Model Can be trained using the MNIST Data. Alternatiely `model.py` file can be imported directly in any another notebook and can be trained on other datasets and saved to the disk.

Standalone, `utils.py` can also be used for the generic train, test and metrics plotting methods irrespective of the notebook file and the model file.