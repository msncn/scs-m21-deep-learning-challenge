# Report

## Overview of the analysis: 

The nonprofit foundation Alphabet Soup wants a tool to help it select the applicants for funding with the best chance of success in their ventures. 

This analysis aims to use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Results: 

Data Preprocessing

* What variable(s) are the target(s) of the final your model?
  * The `IS_SUCCESSFUL` column
* What variable(s) are the features of the final model?
  * Name
  * APPLICATION_TYPE
  * AFFILIATION
  * CLASSIFICATION
  * USE_CASE
  * ORGANIZATION
  * INCOME_AMT
  * ASK_AMT
* What variable(s) have been removed from the input data?
  * EIN
  * SPECIAL_CONSIDERATIONS
  * STATUS

Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your initial neural network model?
  * 2 layers with 80 and 30 neurons
 ![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/b0132526-7de0-4e97-8901-db0eeebe9b65)

* Were you able to achieve the target model performance?
  * No, the accuracy is about 73% and less than the target of 75%
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/fa8d496a-ea81-4463-9be9-b2dc392d5eb0)

* What steps did you take in your attempts to increase model performance?
  * Added a third layer but the output shows 72% which is less than 75%
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/ecf14760-df06-4193-80ba-51eec9d7fecf)
  * Dropped `SPECIAL_CONSIDERATIONS` and `STATUS` but the output still shows 73% which is less than 75%
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/fc24604c-c7ac-49d2-a2ac-cd8217b5fc93)
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/3b6f7825-0c50-49d8-88f8-66eaad6b3638)
 * Added more neurons for the hidden layers but the output shows about 73% still less than 75%
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/5750800e-187b-40fb-8022-bb1b695240de)
 * Adjust `NAME` binning and the output shows 78.5% which is higher than 75%
![image](https://github.com/msncn/scs-m21-deep-learning-challenge/assets/130943141/32fc71d5-713d-4499-ad85-bde6829e2305)

## Summary: 
The neuron network reached 79.5% accuracy. The initial accuracy is about 73% which is less than the target accuracy of 75%. Several attempts were made and achieved by adjusting the name binning.

