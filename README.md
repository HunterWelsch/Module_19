# Module_19

#Questions
1. How many neurons and layers did you select for your neural network model? Why?
Four layers were used when making this model, consisting of an input layer, two hidden layers, and an output layer. The input layer consists of ten input features to match the variables in the dataframe. The hidden layers both use the relu activation function, while the output layer uses the sigmoid activation function.

2. Were you able to achieve the target model performance? What steps did you take to try and increase model performance?
The model's performance topped out at 72.47%, which is under the target performance of 75%. In an attempt to imporve the model's performance various input features were tried. The orginal dataframe has twelve columns, most are pertinent to the analysis. The final model uses ten input features, two columns were dropped. Nine input features, dropping an extra column, were tried instead of ten, to increase the models perfromance. The effect on the performance was minimal and did not reach the 75% target.

3. If you were to implement a different model to solve this classification problem, which would you choose? Why?
For a true/false classification problem, such as this problem, a SVM could be the best option. SVM's are best when dealing with boolean and binary outcomes. Using a SVM over a neural network would make the model less likely to overfit to a specific dataset. 
