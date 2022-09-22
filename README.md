# SpacehipTitanic_Kaggle

This is my solution to the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic). 

The Titanic dataset is a classic dataset for machine learning. It is a binary classification problem, where the goal is to predict whether a passenger survived or not. 



<br>

## Data
The data is split into two groups:
- training set (train.csv) --> used for training, validation and testing
- test set (test.csv) --> for result submission, no labels given
- a template for submission

<br>

## Model
I used two models:
- Boosted Random Forest (XGBoost)   
    SCORE: 0.79120
- Neural Network (Keras)            
    SCORE: 0.77905
(best score so far: 0.87023)

<br>

## Structure
DATA
- raw
    Data provided by Kaggle
- processed
    preprocessed data (versioned data sets)
    can be used for training, validation and testing (*.npy)

MODELS
- models
    pickled models, incl. information about data and performance
- models_overview
    information about the available models and their performance

NOTEBOOKS
- data analysis
    - notebooks for data pre-analysis
- preprocessing
    - preprocessing pipeline of the data
    - processes and saves data of one preprocessing version
- forests
    - training and testing of the random forest models with XGBoost
    - traines and saves model based on data version
- neural_networks
    - training and testing of the neural network models with Keras
    - traines and saves model based on data version

RESULTS
- reuslts: submission files for the Kaggle competition

<br>

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details