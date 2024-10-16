# UTK Face Age detection

The objective is to find the age of people from their images. The data was acquired from [Kaggle](https://www.kaggle.com/datasets/jangedoo/utkface-new).

# Convolutional Neural Network

These are neural networks that are great at processing visual data.

![image](https://media.licdn.com/dms/image/v2/D5612AQGOui8XZUZJSA/article-cover_image-shrink_600_2000/article-cover_image-shrink_600_2000/0/1680532048475?e=1734566400&v=beta&t=fg16P6kVRgMMT4unjXkNYMQq0WMElB1cphywEp9dHmw)

## Convolution layer

Convolutional neural network utilise the convolution layer. This layer preforms the convolution operation, which is essentially an averaging operation over the pixels but each pixel is given a weight on how much each pixel contributes to the average. It helps smoothen the image and makes only the distinct features standout.

## Pooling

Pooling layer performs an aggregate operation (maximum, minimum, average) on he pool of pixels it is currently working on. It reduces the size of the data, and essentially allows us to work with data that maybe most important to us. 

# About the Project

Simple CNN with multiple hiden layers was used to predict the age of the people. Due to exploding gradients I switched to MAE Loss from MSE and, I decided to use pretrained resnet-34 and trained the suffix layers on the dataset. This reduced the testing loss quite a bit.
