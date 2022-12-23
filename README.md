# Neural_Network_Charity_Analysis
## Project Overview
This project was created to develop a neural network to assist in determining which organizations should be considered for funding from AlphabetSoupCharity. Using previously obtained data of organizations that have been awarded or denied funding, the neural network is to be trained on multiple inputs to finally classify future organization requests for funding.

## Results
- Data Processing
  * The data provided shows a column for 'IS_SUCCESSFUL,' and will be the targeted data point for these predictions.
  * There are many data points (features) that will be used as input for the models. Included are:
1. AFFILIATION
2. APPLICATION_TYPE
3. ASK_AMT
4. CLASSIFICATION
5. INCOME_AMT
6. ORGANIZATION
7. SPECIAL_CONSIDERATIONS
8. STATUS
9. USE_CASE

     * The columns for "NAME" and "EIN" have no direct effect on the success/falure rate, and have been excluded from processing.
- Compiling, Training, and Evaluating the Model

  * Initial preparation for the Sequential Neural Network specified 43 input features, into three processing layers that began with 80 neurons and decreased to 30 and 15, and a single output layer.
  * The target performance of 75% accuracy was not met (72.75%).
  * Further testing was done with three dynamic tuned models that statically and dynamically selected inputs, layers, neurons, and activations.
 These attempts yeilded accuracy results of:
    - First Model: 73.49%
    - Second Model: 73.17%
    - Third Model: 73.51%
    
  * Although accuracy was only improved marginally, the total loss of the dynamic deep learning models did offer an excellent decrease in the Loss factor.
  
  ## Summary
  The deep learning model achieved an accuracy of 73% on the test set of data. Should Alphabet Soup want to continue with a neural network to predict the success of potential investments, it is recommended that more data be collected. The dataset used here did not provide any particularly high correlations to the target variable.

More features should be collected such as how long the organization has been in operation for, and how many previous donations they've received in the past (from Alphabet Soup or otherwise).

## Recommendation

For further investigation of these tests, I recommend alternative, non-sequential hyperparameter models. Another means of improving accuracy is to have more datapoints. Although we did not boost success rate to 75%, we have minimized loss using these tuned models.
