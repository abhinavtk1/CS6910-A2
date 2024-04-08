# Part A: Training from scratch

Here I implement a 5 layer CNN network from scratch using PyTorch library and train it using inaturalist dataset. <br>

1. main_part_a.ipynb <br>
This file contains the code of the CNN architecture and training it using our dataset. <br>
The file has been trained in Google Colab/Kaggle where I have taken the dataset from my Google Drive folder. <br>
Dataset link:  https://drive.google.com/drive/folders/1vJqUoTLPd-uXgYR4Kc0vsnisZcF_AJtp?usp=sharing  <br>
Wandb sweep: <br>
&nbsp;&nbsp;&nbsp;&nbsp;{method: bayes <br>
&nbsp;&nbsp;&nbsp;&nbsp;metric: Validation accuracy <br>
&nbsp;&nbsp;&nbsp;&nbsp;goal: Maximize }<br>
**Maximum validation accuracy: 39.67 %** <br>

2. main_part_a_test.ipynb <br>
This file does the testing of our model using the test data. The model trained using the best hyperparameters sweeped from wandb is used for testing. <br>
**Test accuracy: 39.30%** <br>
3 random images from each class in the test folder were plotted along with their actual and predicted name.The plot was logged into wandb. 
