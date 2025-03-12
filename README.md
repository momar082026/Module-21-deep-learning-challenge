# Machine Learning and Neural Networks

# Overview

The purpose of this analysis was to use machine learning and neural networks to create a model that will help Alphabet Soup Foundation to predict applicants that will succeed in their ventures when they received funding. The dataset has applicant information such as identification, application type, industry sector, government organization classification, organization type, status (active or not), income classification, special concideration for application, finding amount requested and effective use of the money.

# Results

# Data Preprocessing

1. The taget variables is: IS_SUCCESSFUL (column), because the whole purpuse of the analysis is to determine whether or not
   the money was spent correctly and achieved it's goals.

2. The features variables are: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "ORGANIZATION", "STATUS", "INCOME_AMT", "SPECIAL_CONSIDERATIONS", and "ASK_AMT".

3. The Variables "EIN" and "NAME" should be removed from the input data because they are neither targets nor features.

# Compiling, Training, and Evaluating the Model

I have selected 80 neurons for my first hidden_layer1 and 30 neurons for my second hidden_layer2.
The number of neurons in my hidden layers (80 and 30) controls the capacity of the model.
I have chosen it because it is a reasonable starting point for experimentation. If I added more neurons, the model can learn faster, but it might also be prone to overfitting. I have chosen the ReLU and Sigmoid activation functions in hidden and output layers because it allows the model to learn faster non-linear patterns in the data. The output layer uses a sigmoid activation function, which is great for binary classification as it outputs a probability score between 0 and 1.

# Model Performance:

loss: 0.5589
Accuracy: 0.7233

I Achieved a model Performance of 73%, which is less than the required 75% target. It tried to increase the models performance by adding a third_hidden_layer of 10 neurons to see if the model accuracy improved. After trying several times, the model's accuraccy did not increase, so I dceided to leave it at the 73% target.

# Summary

The deep learning model achieved an accuracy of 73%, a solid performance but slightly below the target. To improve, we could consider using advanced models like Random Forest or XGBoost, which are effective for classification tasks with structured data. Alternatively, we could continue optimizing the current model by fine-tuning hyperparameters. With further refinement, this model could reach the 75% accuracy target and enhance the Alphabet Soup nonprofit foundation's ability to predict successful funding applicants.
