# deep-learning-challenge

The report should contain the following:
Overview of the analysis: Explain the purpose of this analysis.
 After four models being tested, model 4 which used auto-optimization had the highest accuracy against the test data at .79, surpassing the 75% accuracy goal. With that, it still had a high loss percentage of .53.

The first model had a lower accuracy at .72, but a higher loss percentage of .59. It used 2 hidden layers with 100 neurons each utilizing the ReLU activation, with a Sigmoid activation for the output layer. The choice of ReLU was based on the observation that the data was non-linear.

In the second model, LeakyReLU activation was used to address the issue of dead neurons preventing further learning. The model had 3 hidden layers with 100 neurons each, and a Sigmoid activation for the output layer. While the training accuracy was high at .96, the accuracy against the test data was lower at .60 which is a sign of overfitting.

The third model used the Tanh activation in an attempt to increase model accuracy. It had 3 hidden layers with 50 neurons each, I lowered the neurons to try and avoid overfitting but was unsuccessful. The model accuracy against the test data was lower than model 4 at .67.

Overall, the best performing model was model 4 though it still had a high loss percentage.

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
