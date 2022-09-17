# Machine-Learning-Linear-Regression

# QUESTION 1:

I loaded the dataset and visualized both the test and train dataset. 
The training set indicated a non-linear relationship as well between the x-train and y-train variables. Both training and test dataset show a non-linear relationship between variables. I engineered the features to add non-linearity by taking the 2nd, 3rd, 4th and 5th orders x-train variable (independent variable.)
In trying to find the non-linear relationship between the variables I tried the 2nd order, 3rd order, 4th order, and 5th order basis functions. I decided not to try other higher polynomials because I wanted to avoid overfitting.

The 2nd order basis function as presented by the graph did not not capture the non-linearity 
between the variables, so I decided to try a higher order of 3. The accuracy of this model is very low 6.8% and has a high mean square error of 187.57.
![Screen Shot 2022-09-16 at 10 28 28 PM](https://user-images.githubusercontent.com/89150972/190839244-92fe6cb0-d85a-4038-857e-bae68b52bdb5.png)

The cubic function fitted the training set better than the 2nd order polynomial function. The cubic function model performed better than the 2nd order function model with an accuracy of 46% and mean squared error of 108.03. The model performed better and had a smaller error which is good. I decided to still find out how it fits using the 4th order function.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.36%20PM.png)

The graph from the 4th order function looked very similar to the function from 3rd order and not surprisingly,produced similar accuracy and mean squred error (46% and 107 respectively). Just to have a clear understanding I produced to find the 5th order function and check how it fitted the model.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.44%20PM.png)

The 5th order polynomial fitted the dataset the most but decided not to try higher functions because I did not want my model to overfit the training dataset. The accuracy of the 5th order polynomial was very good (69.5% compared to the other 3 models)
The mean squared error also reduced to 69.515 compared to other models which had higher average least square errors.
![Alt text](https://github.com/aboadia/Machine-Learning-Linear-Regression/blob/main/Screen%20Shot%202022-09-16%20at%2010.28.54%20PM.png)


# QUESTION 2:

I excluded the house ID variable since it was not a feautre. 
Upon fitting the model I observed an average least square error of 38.911.
The results indicates that local_price has the most effect on price, because it has the highest weight or impact on the target value.
Yes,I can use only local price as the target variable becuase it has the most impact.
I am able to determine this by finding the biggest weight or coeffcient from the weights obtained from my model.

The results also indicates that age of home has the least effect on price.
I am able to determine this my finding the least weight or coeffcient, or the weight closet to zero.
After removing the age of home feature the model performed better with an accuracy of 88.88% and a mean square error of 32.13%. The initial model had an accuracy of 86.53% and mean square error of 38.91.

# QUESTION 3: 

There is no need for basis functions when using a locally weighted approach.
Locally weighted linear regression is a non-parametric algorithm, that is, the model does not learn a fixed set of parameters as is done in ordinary linear regression.
Rather parametersor weigths are computed individually for each query point(x). While computing the weights, a higher “preference” is given to the points in the training set lying in the vicinity of the query point than the points lying far away from x.
For polynomial basis functions:
This approach engineers the features and very sentitive to outliers. The polynomial basis function learns a fixed set of parameters. The presence of one or two outliers in the data can seriously affect the results of nonlinear analysis. In addition, 
there are unfortunately fewer model validation tools for the detection of outliers in nonlinear regression than there are for linear regression.
![Screen Shot 2022-09-16 at 10 29 09 PM](https://user-images.githubusercontent.com/89150972/190839200-31517e72-dfbf-4286-b419-10d86ce36061.png)


