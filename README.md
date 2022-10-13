# Neural Network Charity Analysis

## Overview
Alphabet Soup is recognized as a large non-profit philanthropic foundation whose mission is dedicated to helping organizations that protect the environment, improve people’s well-being, and unify the world. The foundation has raised and donated over $10 billion dollars in the past 20 years. The money provided to organizations have gone so far as being used to invest in lifesaving technologies and organization reforestation groups around the world.

Our mission for our project is to utilize neural networks in order to predict which organizations are worth donating to and which ones are categorized as being high risk. Through the use of a mathematical data driven model, we will turn out attention to creating a neural network that we can design and train a deep learning neural network models. The model should provide an accurate output that helps us determine and evaluate which organizations should receive donations from Alphabet Soup. 

The business team has provided a CSV listing more than 34,000 organizations that have received funding rom Alphabet Soup from over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:
- EIN and NAME—Identification columns
- APPLICATION_TYPE—Alphabet Soup application type
- AFFILIATION—Affiliated sector of industry
- CLASSIFICATION—Government organization classification
- USE_CASE—Use case for funding
- ORGANIZATION—Organization type
- STATUS—Active status
- INCOME_AMT—Income classification
- SPECIAL_CONSIDERATIONS—Special consideration for application
- ASK_AMT—Funding amount requested
- IS_SUCCESSFUL—Was the money used effectively

With the raw dataset, we will look to preprocess the data on the csv before training and fitting it into a neural network model and then optimize our model to see if shifting around any components will increase its accuracy. 

## Tools Used:
- Jupyter Notebook
- Python

## Dataset:
- Alphabet Soup Charity Dataset: charity_data.csv

## Results

### Data Preprocessing

**What variable(s) are considered the target(s) for your model?**
The IS_SUCESSFUL is considered to be the target for the model established.

**What variable(s) are considered to be the features for your model?**
The following variables are considered to be features of the model:
- APPLICATION_TYPE
- AFFLICATION
- CLASSIFICATIONS
- USE_CASE
- ORGANIZATION
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT

**What variable(s) are neither targets nor features, and should be removed from the input data?**
The EIN and NAME variables are considered neither targets nor features and are therefore removed from our evaluation and the input data. 

### Compiling, Training, and Evaluating the Model
**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
When it came time to compile and train the model, for the first initial approach, two hidden layers were established. In the first hidden layer, it contained 80 neurons, while the second layer held 30 neurons. In terms of the activation functions selected for the model, both hidden layers utilized the ‘relu’ function while the output later utilized sigmoid. These features were selected as it was believed that it could allow us to achieve a high performance of the model.

**Were you able to achieve the target model performance?**
Ultimately, the model ended up producing an accuracy of 72.66%, which did not achieve the target of obtaining an accuracy of 75% or higher.

**What steps did you take to try and increase model performance?**
To achieve a target predictive accuracy higher than 75%, we sought to increase model performance, we looked to optimize the existing model further by doing the following actions:
- Adding more neurons to the hidden layers
- Adding more hidden layers
- Utilize different activation functions for the hidden layers

Apart from these updates, an additional column, ‘STATUS’ was dropped from the input data as we felt the column had no additive value while it was not a target or feature variable.

## Summary
Despite our three attempts at optimizing the model, accuracy of 75% was not achieve. The highest accuracy performance provided results of 72.54%. Utilizing different features from the original model produced gave greater insight on the smallest optimizations have a big impact on the accuracy produced via the model.

Another model worth exploring that would solve the classification problem is the random forest model type. The random forest has many positive associations as it is considered one of the most powerful model types as they are easy to interpret and can handle outliers and nonlinear data. Also, our data does not contain images or natural language data, which makes using random forest another strong contender. It might allow us to reach the accuracy of 75%, it is worth exploring to create this model and comparing it against the deep learning models we have already established. 





