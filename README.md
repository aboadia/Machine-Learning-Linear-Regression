# Machine-Learning-Linear-Regression

QUESTION 1:
I loaded the dataset and visualized both the test and train dataset. 
The training set indicated a non-linear relationship as well between the x-train and y-train variables. Both training and test dataset show a non-linear relationship between variables. I engineered the features to add non-linearity by taking the 2nd, 3rd, 4th and 5th orders x-train variable (independent variable.)
In trying to find the non-linear relationship between the variables I tried the 2nd order, 3rd order, 4th order, and 5th order basis functions. I decided not to try other higher polynomials because I wanted to avoid overfitting.

The 2nd order basis function as presented by the graph did not not capture the non-linearity between the variables, so I decided to try a higher order of 3. The accuracy of this model is very low 6.8% and has a high mean square error of 187.57.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.28%20PM.png)

The cubic function fitted the training set better than the 2nd order polynomial function. The cubic function model performed better than the 2nd order function model with an accuracy of 46% and mean squared error of 108.03. The model performed better and had a smaller error which is good. I decided to still find out how it fits using the 4th order function.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.36%20PM.png)

The graph from the 4th order function looked very similar to the function from 3rd order and not surprisingly,produced similar accuracy and mean squred error (46% and 107 respectively). Just to have a clear understanding I produced to find the 5th order function and check how it fitted the model.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.44%20PM.png)

The 5th order polynomial fitted the dataset the most but decided not to try higher functions because I did not want my model to overfit the training dataset. The accuracy of the 5th order polynomial was very good (69.5% compared to the other 3 models)
The mean squared error also reduced to 69.515 compared to other models which had higher average least square errors.
![Alt text]()
