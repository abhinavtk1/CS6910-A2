# Part B : Fine-tuning a pre-trained model

I used resnet50 model as the pre-trained model and fine-tune it using the inaturalist data. <br>

1. main_part_b.ipynb <br>
First I loaded the resnet50 model from torchvision.models, then I finetuned it using different types of strategies. Found the best hyperparameters using wandb sweep. <br>
The file has been trained in Google Colab/Kaggle where I have loaded the dataset from my Google Drive folder. <br>
Dataset link:  https://drive.google.com/drive/folders/1vJqUoTLPd-uXgYR4Kc0vsnisZcF_AJtp?usp=sharing  <br>
Wandb sweep: <br>
&nbsp;&nbsp;&nbsp;&nbsp;{method: bayes <br>
&nbsp;&nbsp;&nbsp;&nbsp;metric: Validation accuracy <br>
&nbsp;&nbsp;&nbsp;&nbsp;goal: Maximize }<br>
**Maximum validation accuracy: 79.04%** <br>

2. main_part_b_test.ipynb <br>
This file does the testing of our fine-tuned model using the test data. The model trained using the best hyperparameters sweeped from wandb is used for testing. <br>
**Test accuracy: 75.95%** <br>


