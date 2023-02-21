![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white)

# Multi Class Text Classification

## Data loading 
- uses pandas to read csv file in the dataset folder
- get data from [susanli2016](https://raw.githubusercontent.com/susanli2016/PyCon-Canada-2019-NLP-Tutorial/master/bbc-text.csv)

## Data cleaning
- remove weird symbol and number

## Feature selection
- text is feature 
- categories is target

## Data preprocessing
- using Tokenizer to fit text (change the word to a number)
- using OneHotEncoder to fit category, which is target data (change to 0-4)
- using train test split to split the train and test data

## Model development
- set dim at 256 and droupout rate at 0.3
- using Sequential model
- add embadding as input
- using LSTM and dropout for hidden layer, set 2 hidden layer 
- using Dense softmax activation as output 
- summary of the model ![img](/model.png)

- compile using 'adam' optimizer 
- set tensorboard and early stopping for callbacks and test the model
- the model will stop if there is no more progress in accuracy

## Model analysis
- plot the model result 
 ![img](/accuracy.png)
 ![img](/loss.png)
 

## model prediction 
 - predict the model and test the accuracy
 
 classification report 
 - ![img](/classification_report.png)
 
 confusion matrix
 - ![img](/confusion_matrix.png)
 
 accuracy score and f1_score
 - ![img](/f1_score.png)
 
 
 - [susanli2016](https://raw.githubusercontent.com/susanli2016/PyCon-Canada-2019-NLP-Tutorial/master/bbc-text.csv)
