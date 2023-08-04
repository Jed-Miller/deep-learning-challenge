# deep-learning-challenge

## Charity Fundraising Prediction Model

### Overview

The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. Using machine learning and neural networks, use the features in the provided dataset to create a binary classifier that predicts whether applicants will be successful if funded by Alphabet Soup.

### Data Preprocessing

#### Dropped Columns

**EIN** and **NAME** columns are dropped because they are neither targets or features.

#### Target Variable

**IS_SUCCESSFUL** is the target variable we are trying to evaluate

#### Feature Variables

**APPLICATION_TYPE**<br>
**AFFLIATION**<br>
**CLASSIFICATION**<br>
**USE_CASE**<br>
**ORGANIZATION**<br>
**STATUS**<br>
**INCOME_AMT**<br>
**SPECIAL_CONSIDERATIONS**<br>
**ASK_AMT**<br>

#### Compiling, Training, and Evaluating the Model

The first model was built with the following parameters:

**Input Dimension:** 43<br>
**Hidden Layers:** 2 (80, 30)<br>
**Activation Function:** 2 (relu, relu)<br>
**Output Layer:** 1 (sigmoid)<br>

**Accuracy Score:** 72.1%

Recognizing the first model did not reach the 75% threshold, the second model was built with the following parameters:

**Input Dimension:** 43<br>
**Hidden Layers:** 3 (90, 30, 20)<br>
**Activation Function:** 3 (relu, relu, relu)<br>
**Output Layer:** 1 (sigmoid)<br>

**Accuracy Score:** 72.8%

Recognizing the second model also did not reach the 75% threshold, the third model was built with the following parameters:

**Input Dimension:** 43<br>
**Hidden Layers:** 2 (70, 70)<br>
**Activation Function:** 3 (relu, relu)<br>
**Output Layer:** 1 (sigmoid)<br>

**Accuracy Score:** 72.6%


#### Model Optimization

Lastly, I decided to run an optimization session, and the result that came back was actually the third model that I had run already. Ironically, this model had the worst results of the three models that I had previously run.

#### Summary

After manually setting up three model sessions as well as an optimization session, my analysis is that the data is fairly resist to moving beyond 72-73% accuracy. My next step would be to go back through the data to see what features might be the cause of this lack of elasticity.








