# Deep Learning Model to Evaluate Start Up Success 


Step 1: Preprocess the Data
Compile, train, and evaluate the neural network model.

![image](https://github.com/albertdudek7/Deep_Learning_Model_to_Evaluate_StartUp_Funding/assets/127783844/2e436570-2414-4a6b-a475-44955ace64f3)

Determine the number of unique values for each column.

For columns that have more than 10 unique values, determine the number of data points for each unique value.

Use the number of data points for each unique value to pick a cutoff point to bin "rare" categorical variables together in a new value, Other, and then check if the binning was successful.

Use pd.get_dummies() to encode categorical variables.

Split the preprocessed data into a features array, X, and a target array, y. Use these arrays and the train_test_split function to split the data into training and testing datasets.

Scale the training and testing features datasets by creating a StandardScaler instance, fitting it to the training data, then using the transform function.

![image](https://github.com/albertdudek7/Deep_Learning_Model_to_Evaluate_StartUp_Funding/assets/127783844/f1413c01-947b-4e45-9543-2d0e06f9d40a)

![image](https://github.com/albertdudek7/Deep_Learning_Model_to_Evaluate_StartUp_Funding/assets/127783844/53435a18-390e-4201-9079-8c1cb6cde2fe)


Step 2: Compile, Train, and Evaluate the Model

Create a neural network model by assigning the number of input features and nodes for each layer using TensorFlow and Keras.

![image](https://github.com/albertdudek7/Deep_Learning_Model_to_Evaluate_StartUp_Funding/assets/127783844/1251bf29-08ad-4617-97e4-a1278c9d189a)

Step 3: Optimize the Model
Using your knowledge of TensorFlow, optimize your model to achieve a target predictive accuracy higher than 75%.

![image](https://github.com/albertdudek7/Deep_Learning_Model_to_Evaluate_StartUp_Funding/assets/127783844/250db6e6-ae39-48ab-b281-fe088725b29c)

Step 4: Write a Report on the Neural Network Model
The report should contain the following:

1. Overview of the analysis: Explain the purpose of this analysis.
  The purpose of the analysis is to determine and select funding for applicants with the best chance of success in their ventures. 
  It is to determine the likelihood and predict the probability that an applicant would be successful if they are funded by Alphabet Soup.

2. Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
- The target variable for the model is the 'IS_SUCCESSFUL' column. It is the variable that identifies whether the money was used effectively or not.
What variable(s) are the features for your model?
- All other variables, apart from 'IS_SUCCESSFUL' from application_df were the feature variables of the model. Hence, why 'IS_SUCCESSFUL' was dropped.
What variable(s) should be removed from the input data because they are neither targets nor features?
- 'EIN' and 'NAME' columns were both removed from the dataset because they were neither targets nor features.


Compiling, Training, and Evaluating the Model

1.How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - For the initial neural network model I choose to use 10 hidden_node_layers1 and 5 hidden_node_layers2.
  - I used tanh as an activation function for the first hidden layer, relu as the activation function for the second hidden layer and relu for the output layer.
  - The reason I choose 10 and 5 respectively for the hidden_node_layers was it was the number used in some class activities. Similarly, using tanh and relu was found to be accurate in other examples as well. 

2. Were you able to achieve the target model performance?
  - I was not able to achieve the target model performance of 75% but was relatively close at 72.3% tested using 20 epochs. 

3. What steps did you take in your attempts to increase model performance?
  - I made significant changes to increase model performance. To begin with, I added an additional third hidden layer to the model. 
  - I kept the number of nodes for the first hidden layer the same, but increased the nodes for the second hidden layer to 8 and set the number of nodes for the newly added third layer to 6. 
  - I decided to use a relu activation function instaed of tanh for the first hidden layer, and sigmoid as the activation function for the second, third and output layers. 
  - Lastly, I slightly increased the number of epochs to 25 from 20. This was signicant and interestingly using a higher number of epochs (ie: 40) led to decreased accuracy. 


3. Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
  - The overall results of the first model yielded accuracy of 72.3% and the optimized model yielded an improved accuracy of 77.0%. 
  - A few recommendations be test different activation functions to determine which produces a greater correlation between input and output. A higher correlation between input and output most likely produces higher accuracy.
  - In this instance, increasing the number of nodes for hidden layer 2 may have been linked to an increase in accuracy.
  - Additionally, (slightly) increasing the number of epochs led to increased accuracy as well. 
