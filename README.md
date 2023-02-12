# Neural_Network_Charity_Analysis
### Overview
This project uses the features in the provided dataset to create a binary classifier that is capable of predicting whether loan applicants will be successful if funded by Alphabet Soup.

From Alphabet Soup’s business team, a CSV containing more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization, such as the following:

    EIN and NAME—Identification columns
    APPLICATION_TYPE—Alphabet Soup application type
    AFFILIATION—Affiliated sector of industry
    CLASSIFICATION—Government organization classification
    USE_CASE—Use case for funding
    ORGANIZATION—Organization type
    STATUS—Active status
    INCOME_AMT—Income classification
    SPECIAL_CONSIDERATIONS—Special consideration for application
    ASK_AMT—Funding amount requested
    IS_SUCCESSFUL—Was the money used effectively


### Results
#### Data Preprocessing
What variables are considered the target(s) for the model?
- The 'IS SUCCESSFUL' variable would be the target for the model. We are trying to predict if the loan borrower will repay their loan in time.

What variables are considered to be the features for your model?
- Application Type
- Affiliation
- Classification
- Income AMount
- Asking Amount

What variables are neither targets nor features and should be removed from the input data?

After doing further tests, the following variables do not have significant impact on the output of the model and should be removed:
- EIN and NAME
- USE_CASE
- ORGANIZATION
- STATUS
- SPECIAL_CONSIDERATIONS

#### Compiling, Training, and Evaluating the Model
How many neurons, layers and activation functions did you select for your neural network?
- For the initial model, two layers were built. The first layer used 80 nodes, and the second used 30 nodes. The activation function implemented was relu. This format was used as suggested best practice for the data provided. Note: For this and all following models, the number of nodes selected was arbitrary, based on previous experience with building models.
- The first optimization model used two layers. The first layer was expanded to use 100 nodes with the second using 30 nodes. The activation function implemented was relu. This model was attempted in order to see if increasing the number of nodes in the first layer would improve the performance of the model.
The second optimization model used three layers. The first layer implemented 80 nodes, the second 30, and the third 10 nodes. The activation function implemented was relu. This model was attempted in order to see if a third layer of nodes would increase the performance of the model.
The third optimization model used two layers. The first layer implemented 80 nodes, the second 30 nodes. The activation function implemetned was tanh. This model was attempted to see if modifying the activation function would improve the performance of the model.
Were you able to achieve the target model performance?
- The target performance of 75% was not met in any of the three models built.
What steps did you take to try and increase model performance?
- There were multiple steps including increasing the nodes in the hidden layer, increasing the number of overall layers and changing the activation function.

### Summary

The target performance threshold of 75% was not met. Each model fell just short of the goal.
- Initial Model - 73.12%
- Optimization Model 1 - 72.97%
- Optimization Model 2 - 72.82% 
- Optimization Model 3 - 72.70%

In order to meet the goal, further optimization must be done on the models like changing the activation function and removing and refining the columns. 
