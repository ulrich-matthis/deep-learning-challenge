AlphabetSoup Neural Network Data Analysis

Analysis Overview:
The purpose of our anlysis is to determine how accurately we can determine whether bids for financial assistance will be successful or unsuccessful. Using skills learned in this module neural networks were created and the goal was to predict with a 75% accuracy whether projects would be successful or unsuccessful. For the creation of our model we examined AlphabetSoup financial data removed unwanted columns (EIN and Business Names) and scaled and transformed the remaining data to help train our model to provide assistance in predicting future success of future clients based on our current sample size.

Results:
Data Preprocessing

What variable(s) are the target(s) for your model?
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?

- Our target variable for our analysis was the "IS_SUCCESSFUL" column.
- Our feature variables for this analysis were application type, affiliation, classification, use case, organization type,
status, income, special considerations and ask amount.
- EIN and Name were initially removed during our preprocessing as they were not pertinent to our model

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?

- For the control model I used two hidden layers with 7 and 4 neurons respectively. For our best optimization model I used 4 hidden layers with 8, 5, 6 and 5 neurons with tanh being used on the first three layers and relu on the final layer.
- I was unable to achieve the target performance with my model; however, I was able to achieve marginal gains on both loss and accuracy
- Lower numbers of epochs and an extra hidden layer helped to provide these small gains along with using both tanh and the relu activation functions.

Summary:

The results of our modeling, as stated above were not able to reach the desired results even with the addition of extra hidden layers and tweaks to the activations for the hidden layers. The best score recorded:

loss: 0.5544  accuracy: 0.7262

Some further adjustments that could have been made to assist our model would be to further trim down our data features to see if any of the other included columns following preprocessing were causing any unforseen interference for our model. Another suggestion would be to use the available keras tuner to provide additional developer assistance with the creation of this model in a more streamlined manner.
