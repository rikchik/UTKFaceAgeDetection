# UTK Face Age detection

The objective is to find the age of people from their images. The data was acquired from [Kaggle](https://www.kaggle.com/datasets/jangedoo/utkface-new).

Simple CNN with multiple hiden layers was used to predict the age of the people. Due to exploding gradients I switched to MAE Loss from MSE and, I decided to use pretrained resnet-34 and trained the suffix layers on the dataset. This reduced the testing loss quite a bit.
