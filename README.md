# Machine_Learning
Types of Machine Learning:

#### 1. Regression
#### 2. Classification
#### 3. Clustering

#### 1. Regression:- 
Output variable predicted on the basis of past data over continuous/numeric dataset resulted to a continuous variable.
for example- 
1.creating merit list for qualified students for Post graduation Programs on the basis of graduation score.
2.You have a dataset of BMI (body mass index) and the fat percentage of the customers of a fitness centre. Now, the fitness centre wants to predict the fat percentage of a new customer, given his BMI.
3.You want to predict the sales of a retail store based on its size, given the dataset of sales of retail stores and their sizes.

#### 2. Classification:- 
Output variable predicted on the basis of past data over categorical/label dataset resulted to a categorical variable.
for example:-
1.Classifying emails on the basis of subjectline/content.
2.A Singapore-based startup Healin launched an app called JustShakeIt, which enables a user to send an emergency alert to emergency contacts and/or caregivers simply by shaking the phone with one hand. The program uses a machine learning algorithm to distinguish between actual emergency shakes and everyday jostling, using data with labels.
3.You have collected data from a house rental website like commonfloor.com. The data has the rental prices of apartments and customer ratings as HIGH or LOW. You want to predict the customer rating, given the rental price of a new house.
4.You want to predict whether a customer is likely to leave the telecom network

#### 3. Clustering:-  
Output Variable predicted on the basis of large amount of data over without labeled dataset resulted to a categorical                    variable after analysis, for example- customer segmentation on the large amount of customer dataset

##### *----Point To be Noted---*
1.Regression and Classification Comes under Supervised Learning
2.In both of them we have Labels
3.Regression has Continuous/numeric labels  in dataset
4.Classification has Categorical Labels in dataset
5.Both gives result on the basis of Past behaviour of dataset.

##### *----Point to be Noted---*
1.Clustering Comes under Un-Supervised Learning
2.it doesn't have labels and here we have large amount of dataset 
3.Result comes as a categorical variable after analysis.

##### *----Point to be Noted---*
Predictive analysis is used to build the model on training data and the we predict on the test data if our model has passed the tests.


### Linear Regression Line:-
1.The equation of a straight line is usually written this way:
#### y = mx + b
![Capture1](https://user-images.githubusercontent.com/16449922/60673158-c2ad5a80-9e94-11e9-9e1e-f991ef37c201.JPG)

#### Linear regression models can be classified into two types depending upon the number of independent variables:-

##### Simple linear regression: When the number of independent variables is 1
##### Multiple linear regression: When the number of independent variables is more than 1


#### 2.Slope(m)=(y2-y1)/(x2-x1)
#### 3.Intercept= b

##### Ques-
The independent variable X from a linear regression is measured in miles. If you convert it to kilometres (keeping the unit of the dependent variable Y the same), how will the slope coefficient change? (Note: 1 mile = 1.6 km)
##### Ans-
It will get divided by 1.6.
In the linear regression equation, X gets multiplied by 1.6 with no change in Y. So, the slope will be divided by 1.6.


5.Machine Learning Standard Notation for Straight line:
#### y=β0+β1x

4.For fitting the best line in Scatter Plot
We find out Residuals

#### Residual(ei)=yi-ypred

here ei is the error at a particlar datapoint

yi is the actual value at that data point

ypred is the predicted value at a particular datapoint

To minimize the error here we use ordinary least squares method-
![Capture3](https://user-images.githubusercontent.com/16449922/60716446-09568f80-9f3d-11e9-8e41-94ff5f693a25.JPG)

#### The equation of the best fit regression line Y = β₀ + β₁X can be found by minimising the cost function (RSS in this case, using the Ordinary Least Squares method) which is done using the following two methods:

##### Differentiation
##### Gradient descent method

#### Gradient Descent
Gradient descent is an optimization algorithm used to find the values of the parameters (coefficients) of a function (f) that minimizes a given cost function (cost).
 
Recall the equation for the line that's fit the data, is given as:
y=β0+β1x
Where β0 is the intercept of the fitted line and 
β1 is the coefficient for the independent variable x.

we need to reduce the cost function for all data points, which is given as,

![Capture4](https://user-images.githubusercontent.com/16449922/60717899-d910f000-9f40-11e9-8cad-d97c05fc0208.JPG)

Gradient Descent approach is one optimization technique to find β0,β1 so that cost function is minimized/Optimized.
There are two types of Optimisation methods,

##### Closed form solution
##### Iterative form solution

Here Gradient descent is an iterative form solution of order one. So to compute optimal thetas, we need to apply Gradient Descent to the Cost function, which is given as follows,

![Capture1](https://user-images.githubusercontent.com/16449922/60719054-217ddd00-9f44-11e9-95e1-c3c37ddd7fef.JPG)

#### Closed Form Solution:-

![Capture1](https://user-images.githubusercontent.com/16449922/60719054-217ddd00-9f44-11e9-95e1-c3c37ddd7fef.JPG)

J'(x)=0
2x=0
x=0
then x(optimized)=0

#### Iterative Form-(First Order):-
Gradient descent is an iterative method of optimising an objective function, in our case the cost function, by moving toward the negative of the gradient.

 To compute θ1, the equation :-
 
 ![Capture2](https://user-images.githubusercontent.com/16449922/60720976-0c0bb180-9f4a-11e9-8593-c9907f2ee7a5.JPG)

Where η is known as the learning rate, which defines the speed at which we want to move towards negative of the gradient. ​

##### *---Point to be noted---*
A large value of learning rate may oscillate your solution, and you may skip the optimal solution(global minima). So it's always a good practice to choose a small value of learning rate and slowly move towards the negative of the gradient.

##### R-Squared,TSS and RSS
![Capture3](https://user-images.githubusercontent.com/16449922/60733038-5d776900-9f69-11e9-8332-b7c4ec9ee2d5.JPG)

##### *---Point to be Noted---*
The fit becomes better and better when R-Squared value is close to 1 or 1 ,i.e. if residuals are zero the R-Squared is 1

#### The strength of a linear regression model is mainly explained by R²,  where R² = 1 - (RSS / TSS)
##### RSS: Residual Sum of Squares
##### TSS: Total Sum of Squares


#### Apart from R², there is one more quantity named RSE (Residual Square Error) which is linked to RSS. 

![Capture4](https://user-images.githubusercontent.com/16449922/60734455-acbf9880-9f6d-11e9-9a56-273bfcb68a4e.JPG)

final assumed true Linear Relationship:-
y=β0+β1x+e

e is some error

![Capture2](https://user-images.githubusercontent.com/16449922/60738546-53ab3100-9f7c-11e9-8c8d-a24ec185236b.JPG)

Now 
 
![Capture1](https://user-images.githubusercontent.com/16449922/60738619-9836cc80-9f7c-11e9-9563-a1bfd75d8979.JPG)

where β0 & β1 with a hat notion represents that these are estimated values

