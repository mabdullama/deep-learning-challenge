# Charity Neural Model Funding Analysis

## Overview of the analysis
The nonprofit foundation *Alphabet Soup* wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With  knowledge of machine learning and neural networks, we’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup. The dataset is a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years.

## Data Preprocessing
* Target: 
    * IS_SUCCESSFUL

* Features:
    * APPLICATION_TYPE
    * AFFILIATION
    * CLASSIFICATION
    * USE_CASE
    * ORGANIZATION
    * INCOME_AMT
    * ASK_AMT
    * IS_SUCCESSFUL

* Variables to be removed:
    * EIN
    * NAME
    * STATUS
    * SPECIAL_CONSIDERATIONS

## Compiling, Training, and Evaluating the Model
* The model consit of three layers total for with 75 nodes run for 100 epochs was used to create the model. After significant trial an error, this combination gave the highest accuracy score 73% accuracy which was under a desired 75% but not too far off.

* What steps did you take in your attempts to increase model performance?
 In order to increase the system performance I added one more hidden layer with 10 nodes  I also tried different activation methodes and changed the number of nodes in the hidden layers, as well as changinging the epochs number to 200 (which increased the compiling time of the model). The optimized model was able to achieve accuracy of 73% and loss of 55%.

## Summary

Although not reaching the 75% accuracy threshold requested, 73% accuracy might be a reasonable percentage  in predicing charity fundraising success.

The dataset does not provide clear insights into the significance of application types or classifications. Also, with a dataset consits 12 columns, there is a lot of information that might not be realted with create more noise in the model . For future research, highlighting  the most important variables could be more benefecial prior to building a neural network. This approach would enable us to focus solely on evaluating the most pertinent factors.