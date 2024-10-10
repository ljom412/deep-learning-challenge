# deep-learning-challenge

# OVERVIEW
The purpose of this challenge was to create a binary classifier using machine learning and neural networks that can predict whether applicants for Alphabet Soup funding will be successful if funded. We were given information on 30,000+ organizations that have received funding from Alphabet Soup in the past, including the organizations' affiliation, classification, use-case, and income amount. We were tasked with preprocessing and scaling the data, compiling and training the neural network model, and then attempting to optimize to achieve a target predictive accuracy higher than 75%.

# RESULTS
**Data Preprocessing**

**What variable(s) are the target(s) for your model?**
  - 'IS_SUCCESSFUL'

  ![alt text](https://github.com/ljom412/deep-learning-challenge/blob/main/Images/target_variable.png?raw=true)

**What variable(s) are the features for your model?**
 - 'APPLICATION_TYPE'
 
 - 'ORGANIZATION' 
 
 - 'CLASSIFICATION' 
 
 - 'AFFILIATION' 
 
 - 'USE_CASE'

![alt text](https://github.com/ljom412/deep-learning-challenge/blob/main/Images/feature_variables.png?raw=true)
  
**What variable(s) should be removed from the input data because they are neither targets nor features?**
  - 'ASK_AMT'

  - 'SPECIAL_CONSIDERATIONS'

**Compiling, Training, and Evaluating the Model**

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**
 
 **Initial Model**

- Two Hidden Layers

- 8 Nodes in First Layer

- 5 Nodes in Second Layer

- Used Rectified Linear Unit Activation Function

![alt text](https://github.com/ljom412/deep-learning-challenge/blob/main/Images/first_model1.png?raw=true)

![alt text](https://github.com/ljom412/deep-learning-challenge/blob/main/Images/first_model2.png?raw=true)

**Most Successful Model**

- Four Hidden Layers

- 20 Nodes in First Layer

- 15 Nodes in Second Layer

- 15 Nodes in Third Layer

- 20 Nodes in Fourth Layer

- Used Hyperbolic Tangent Activation Function
  
**Were you able to achieve the target model performance?**

  No, the highest accuracy I was able to achieve was 66%.

  ![alt text](https://github.com/ljom412/deep-learning-challenge/blob/main/Images/best_accuracy.png?raw=true)
  
**What steps did you take in your attempts to increase model performance?**

  I tried several methods to increase performance: dropping columns, creating more bins for rare occurences in columns, adding more neurons and hidden layers, using different activation functions for the hidden layers, and reducing the number of epochs in the training       regimen.

  # SUMMARY
  Overall, I was able to improve the model's accuracy from about 50% to 66% after 5 attempts at optimization. It's possible that a different model, such as a Random Forest classifier, could perform better with the given dataset. Since Random Forest builds multiple           decision trees and merges them together, it could help improve the model's performance on minority classes. It also provides information on feature importance, so we could see which variables contribute most to the predictions. In this same vein, we could attempt to       apply Principal Component Analysis to the dataset to try to improve accuracy using the more heavily weighted features. Random Forest can also handle both categorical and numerical data, cutting out the need for preprocessing.
