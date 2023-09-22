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
For this part of the assignment, you’ll write a report on the performance of the deep learning model you created for Alphabet Soup.

The report should contain the following:

Overview of the analysis: Explain the purpose of this analysis.

Results: Using bulleted lists and images to support your answers, address the following questions:

Data Preprocessing

What variable(s) are the target(s) for your model?
What variable(s) are the features for your model?
What variable(s) should be removed from the input data because they are neither targets nor features?
Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
Were you able to achieve the target model performance?
What steps did you take in your attempts to increase model performance?
Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
Step 5: Copy Files Into Your Repository
Now that you're finished with your analysis in Google Colab, you need to get your files into your repository for final submission.

Download your Colab notebooks to your computer.

Move them into your Deep Learning Challenge directory in your local repository.

Push the added files to GitHub.
