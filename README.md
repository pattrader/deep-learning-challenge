# deep-learning-challenge (REPORT)

Analysis Report:

Overview of the Analysis:
The purpose of this analysis was to build a deep learning model for a classification problem. The goal was to predict the success or failure of a specific application based on various features.

Results:

Data Preprocessing:

Target Variable(s): The target variable for the model is 'IS_SUCCESSFUL', which indicates whether the application was successful or not.
Feature Variable(s): The feature variables for the model are the remaining columns in the dataset after dropping 'EIN' and 'NAME'.
Variables to Remove: The 'EIN' and 'NAME' columns were removed from the input data as they are neither targets nor features.

Compiling, Training, and Evaluating the AlphabetSoupCharity Model:

Neurons, Layers, and Activation Functions: The neural network model used in this analysis had 70 neurons in the first hidden layer, 35 neurons in the second hidden layer, and a single neuron in the output layer. The activation function used was 'relu' for the hidden layers and 'sigmoid' for the output layer. This configuration was chosen to introduce non-linearity and to optimize the model's performance for binary classification tasks.
Target Model Performance: The target model performance was to achieve a high accuracy in predicting the success or failure of the application. The exact target accuracy is not mentioned in the provided information.
Steps Taken to Improve Model Performance: The provided information does not specify the steps taken to improve model performance. It's possible
that further experimentation and optimization were performed, but the details are not included.

Compiling, Training, and Evaluating the AlphabetSoupCharity_Optimization Model:

Neurons, Layers, and Activation Functions: The model architecture is now created using a hyperparameter tuning approach using Keras Tuner. The number of neurons, layers, and activation functions are determined by the tuner. The tuner is set up to search for the optimal architecture based on the given range of values for neurons and layers and the choice of activation functions.
Target Model Performance: The target model performance is not explicitly defined in the code. However, the tuner is set to optimize the model based on the "val_accuracy" metric, which is the validation accuracy.
Steps Taken to Improve Model Performance: The code implements hyperparameter tuning using the Hyperband algorithm from Keras Tuner. The tuner performs a search for the best hyperparameters, including the number of layers, number of neurons, and choice of activation functions, to optimize the model's performance. It also evaluates the model on the validation data during the search process.

The deep learning model achieved a loss of approximately 0.5521 and an accuracy of approximately 0.7314. While the model achieved a decent accuracy, further evaluation and analysis are required to determine if it meets the target performance.The updated code incorporates hyperparameter tuning using Keras Tuner to optimize the deep learning model's architecture. The tuner searches for the best combination of activation functions, number of layers, and number of neurons to achieve the highest validation accuracy. This approach allows for better model performance by exploring a wider range of possible architectures.

Please note that specific performance metrics, such as the final accuracy achieved by the optimized model, are not provided in the code. You may need to run the code and evaluate the model to obtain those specific results.

Recommendation for a Different Model:
A different model that could potentially solve this classification problem is a Random Forest classifier. Random Forest is an ensemble learning algorithm that combines multiple decision trees to make predictions. It has the ability to handle a large number of features and can handle both numerical and categorical data without requiring extensive preprocessing. It also provides feature importance analysis, which can help identify the most influential factors in predicting the success of an application.

The recommendation for a Random Forest classifier is based on the potential benefits it offers, such as robustness, interpretability, and the ability to handle complex datasets. However, further evaluation and experimentation would be necessary to determine if it outperforms the deep learning model in terms of accuracy and other performance metrics.
