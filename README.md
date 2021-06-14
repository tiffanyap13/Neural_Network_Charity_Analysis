# Neural Network Charity Analysis

## Overview of the analysis
With my knowledge of machine learning and neural networks, I used the features in the provided dataset to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. Alphabet Soup is a charitable organization that is dedicated to helping other organizations protect the environment. 

Alphabet Soup’s business team shared a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization.  The purpose of this project is to ensure that that the donation monies are allocated wisely to the most impactful organizations.

## Results
### Variables
 - The variable considered to be the target for the model is IS_SUCCESSFUL.
 - The variables that are considered to be the features for the model are the following:
     - APPLICATION_TYPE
     - AFFILIATION
     - CLASSIFICATION
     - USE_CASE
     - ORGANIZATION
     - STATUS
     - INCOME_AMT
     - SPECIAL_CONSIDERATIONS
     - ASK_AMT
 - The variables that are neither targets nor features, and were removed from the input data, are EIN and NAME.
 ### Compiling, Training, and Evaluating the Model
 - I selected the following: neurons (81, 31, 10), three layers, and two activation functions (relu and sigmoid) for the neural network model.  The neurons were selected randomly and modified to increase the performance result, as were the number of layers.  The activation functions were selected to increase efficiency and effectiveness of learning. Relu is known for allowing models to learn faster and perform better. Sigmoid is great to use for models where we have to predict the probability as an output. 
 - I was able to achieve the target model performance at 99.9%.
 - The steps I took to try and increase model performance including the addition of a layer, changing the third layers neurons, and also adjusting the epochs.

## Summary
The overall results of the deep learning model were successful at 99.9%.  However, there is a slight concern that the model was overtrained since its accuracy is extremely high. 

A recommendation for a different model to use is logistic regression.  A logistic regression model is a classification algorithm that can analyze continuous and categorical variables. Using a combination of input variables, logistic regression predicts the probability of the input data belonging to one of two groups. If the probability is above a predetermined cutoff, the sample is assigned to the first group, otherwise it is assigned to the second. For example, using an applicant's information, logistic regression could be used by Alphabet Soup to determine if the applicant does not qualify for an allocated donation.

