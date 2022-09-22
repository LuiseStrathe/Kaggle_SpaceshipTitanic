# SpacehipTitanic_Kaggle

This is my solution to the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic). 

The Titanic dataset is a classic dataset for machine learning. It is a binary classification problem, where the goal is to predict whether a passenger survived or not. 



<br>

## Data

The Titanic dataset is one of the most popular datasets for beginners in machine learning. The goal of this project is to predict whether a passenger on the Titanic survived or not. The data is split into two datasets, a training dataset and a test dataset (which is for the later rating). The training dataset contains the labels, i.e. whether the passenger survived or not. The test dataset does not contain the labels, and the goal is to use the training dataset to train a model that can predict the labels for the test dataset.

The data used in this project can be found on Kaggle: https://www.kaggle.com/c/titanic/data
The data is split into two groups:
- training set (train.csv) --> used for training, validation and testing
- test set (test.csv) --> for result submission, no labels given
- a template for submission

<br>

## Model

I used the following machine learning methods:
(scores shown are from KAGGLE rank)

Boosted Random Forest   XGBoost     SCORE: 0.79120
Deep Neural Network     KERAS       SCORE: 0.77905

The code is written in python and uses pandas and numpy for data manipulation and scikit-learn for the machine learning algorithms.
<br>

## Structure
DATA
- raw
    - train.csv contains the training data
    - test.csv contains the test data
    - sample_submission.csv is a template
- preprocessed  
    - Contains already preprocessed data 
    - Numpy-arrays are direct inputs for the models

MODELS
- prediction overview
    - contains info about model performance 
    - accuracy is based on test data (from train_csv)
    - corresponding to the saved models
- models        
    - pickeled model versions

NOTEBOOKS
- data_analysis
    - pre-viewing and analysis of data 
    - testing of preprocessing pipeline
- preprocessing
    - contains preprocessing pipeline
    - ensures the equal preprocessing of one data version
    - avoids data leakage
    - TRAIN-csv --> train, val and test set
    - TEST-csv --> generation of results for submission
    - saves a new data version
- forests
    - XGB random forests model
    - run on specific data version from file
    - model saved with training info
- NN_keras
    - Deep Neural Network 
    - build with Tensorflow and keras
    - model saved with training info
- results
    - generates a submission file 
    - based on a chosen model and preprocessing version

<br>

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details





