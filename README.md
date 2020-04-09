# Module_19

## Overview 
Using a neural network to create a binary classifier to predict whether or not an applicant will be successful if funded by the venture capital group.

Input data:
Consists of metadata of 34,000 organizations that have received various amounts of funding from the firm in the past. Includes data from the application process to post funding results. 

Goals:
* Import, analyze, clean, and preprocess the input dataset.
* Select, design, and train a binary classification model.
* Optimize model training and input data to achieve a target predictive accuracy of at least 75%.

Tools/ Languages used:
* Python
* Pandas
* Matplotlib
* Sklearn
* Tensorflow

## Analysis

### Preprocessing
* Specify the target variables and the feature variables
* Encode categorical variables 
* Split data into train/ test sets
* Standardize the data using StandardScaler

### Model
Used a logistic classifier to predict desired outcome.

Neural Network consisted of:
* Four layers:
  * Input layer
  * Two hidden layers with relu activation functions
  * Output layer with sigmoid activation function
* Compiled the model with a binary cross-entropy loss metric and an adam optimizer

## Questions

1. How many neurons and layers did you select for your neural network model? Why?
Four layers were used when making this model, consisting of an input layer, two hidden layers, and an output layer. The input layer consists of ten input features to match the variables in the dataframe. The hidden layers both use the relu activation function, while the output layer uses the sigmoid activation function.

2. Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
The model's performance topped out at 72.47%, which is under the target performance of 75%. In an attempt to improve the model's performance various input features were tried. The original dataframe has twelve columns, most are pertinent to the analysis. The final model uses ten input features, two columns were dropped. Nine input features, dropping an extra column, were tried instead of ten, to increase the models performance. The effect on the performance was minimal and did not reach the 75% target.

3. If you were to implement a different model to solve this classification problem, which would you choose? Why?
For a true/false classification problem, such as this problem, a SVM could be the best option. SVM's are best when dealing with boolean and binary outcomes. Using a SVM over a neural network would make the model less likely to overfit to a specific dataset. 
