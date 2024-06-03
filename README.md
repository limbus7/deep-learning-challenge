# Alphabet Soup Funding Final Analysis

# Purpose

This project uses a deep learning model, to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. 

# Analysis

FIRST MODEL: 

The first model had a lower accuracy at 0.72, but a higher loss percentage of 0.56. It used 2 hidden layers with 8 and 5 neurons each utilizing the ReLU activation, with a Sigmoid activation for the output layer. 
<img width="940" alt="Screenshot 2024-06-03 at 1 05 47 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/bd16154a-0c1a-41c3-85b3-69a4a969da7c">

<img width="1416" alt="Screenshot 2024-06-03 at 1 06 22 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/c9e48069-2149-4a5d-8591-b60e1a8cb9ee">





SECOND MODEL: 

In the second model, 'NAME' colums was dropped, and it used  3 hidden layers with 50 neurons each utilizing the 'ReLU' activation and  a Sigmoid activation for the output layer.The accuracy against the test data was lower at 0.729 with the loss percentage of 0.56. Even after adding the third layer and changing the neurons, the second model did not show much change in the accuracy and loss percentage. 

<img width="1460" alt="Screenshot 2024-06-03 at 1 08 37 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/c74867ee-d539-4032-b01e-eabf5f9f56a4">


<img width="1469" alt="Screenshot 2024-06-03 at 1 09 43 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/88b1f515-0aa9-40a6-a416-48e5d4a11f90">




THIRD MODEL: 
For the third model dropped 'EIN' column only. Three hidden layers were used with 100 neurons each utilizing 'LeakyReLU' activation function. I decided to use 'LeakyReLU' activation function as I could not see much changes in Accuracy and Loss percentaged in the first two models. The accuracy result was 0.59 which was even lesser than the previous models tested and way lesser than the target accuracy percentage.  The high loss percentage of 0.711 which was very high of all the models tested. 



<img width="981" alt="Screenshot 2024-06-03 at 1 10 56 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/52a3804e-3b3c-4d50-84c4-d586189228c1">

<img width="972" alt="Screenshot 2024-06-03 at 1 11 25 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/5c367e30-d0d4-46e3-88c1-d157ec412441">





FOURTH MODEL: 
Finally on fourth model, I was able to achieve accuracy of 0.79 which met the target accuracy of 75% with a loss of 0.57 which is still a very high loss percentage. Since the above 3 optimization model were not able to achieve higher than 75% accuracy, I decided to use Auto-Optimization Model. I chose auto-optimization to get the best model and hyperparameters to obtain accuracy higher than 75%.  This model has 3 layers, with the first layer having 4 neurons and the remaining layers having 6, 6, 7, 7 neurons respectively. The activation function used throughout this model is 'tanh'. 

<img width="1035" alt="Screenshot 2024-06-03 at 1 12 46 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/d9082703-3825-4fd2-901f-f6ad577f32e9">

<img width="1059" alt="Screenshot 2024-06-03 at 1 13 12 AM" src="https://github.com/limbus7/deep-learning-challenge/assets/105176210/4213fbc0-56c2-44b2-8091-79baba956ee1">




# Data Preprocessing

What variable(s) are the target(s) for your model?
The target for each model was the IS_SUCCESSFUL column. 

What variable(s) are the features for your model?
The available features for my model are: EIN, NAME, APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT

What variable(s) should be removed from the input data because they are neither targets nor features?
As instructed I removed EIN and NAME column, the removed column did not make any impact on improving the performance of the model. So I just removed EIN column from the second model till the fourth model with different numbers of neurons and activiation function, I was able to see some difference after adding the NAME column. 



