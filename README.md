# deep-learning-challenge

# OVERVIEW
The purpose of this challenge was to create a binary classifier using machine learning and neural networks that can predict whether applicants for Alphabet Soup funding will be successful if funded. We were given information on 30,000+ organizations that have received funding from Alphabet Soup in the past, including the organizations' affiliation, classification, use-case, and income amount. We were tasked with preprocessing and scaling the data, compiling and training the neural network model, and then attempting to optimize to achieve a target predictive accuracy higher than 75%.

# RESULTS
**Data Preprocessing**

**- What variable(s) are the target(s) for your model?**
  The target variable is the 'IS_SUCCESSFUL' column, which tells us whether the previous organizations were succesfful upon receiving funding from Alphabet Soup.
  
**- What variable(s) are the features for your model?**
  The feature variables included 'APPLICATION_TYPE', 'ORGANIZATION', 'CLASSIFICATION', 'AFFILIATION', and 'USE_CASE'.
  
**- What variable(s) should be removed from the input data because they are neither targets nor features?**
  While attempting to optimize the model to achieve the target accuracy score, I dropped the 'ASK_AMT' and 'SPECIAL_CONSIDERATIONS' variables.

**Compiling, Training, and Evaluating the Model**

**- How many neurons, layers, and activation functions did you select for your neural network model, and why?**
  For the initial model, I used two hidden layers, the first containing 8 nodes and the second containing 5 nodes. I used the rectified linear unit activation function. I chose this as a starting point because I did not want to make the model overly complex before seeing    how it performed the first time.
  
**- Were you able to achieve the target model performance?**
  No, the highest accuracy I was able to achieve was 66%.
  
**- What steps did you take in your attempts to increase model performance?**
  I tried several methods to increase performance: dropping columns, creating more bins for rare occurences in columns, adding more neurons and hidden layers, using different activation functions for the hidden layers, and reducing the number of epochs in the training       regimen.

  # SUMMARY
  Overall, I was able to improve the model's accuracy from about 50% to 66% after 5 attempts at optimization. It's possible that a different model, such as a Random Forest classifier, could perform better with the given dataset. Since Random Forest builds multiple           decision trees and merges them together, it could help improve the model's performance on minority classes. It also provides information on feature importance, so we could see which variables contribute most to the predictions. In this same vein, we could attempt to       apply Principal Component Analysis to the dataset to try to improve accuracy using the more heavily weighted features. Random Forest can also handle both categorical and numerical data, cutting out the need for preprocessing.
