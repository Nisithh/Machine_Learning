# Machine_Learning
Types of Machine Learning:

#### 1. Regression
#### 2. Classification
#### 3. Clustering

#### 1. Regression:- 
Output variable predicted on the basis of past data over continuous/numeric dataset resulted to a continuous variable.
for example- creating merit list for qualified students for Post graduation Programs on the basis of graduation score.

#### 2. Classification:- 
Output variable predicted on the basis of past data over categorical/label dataset resulted to a categorical variable.
for example:-Classifying emails on the basis of subjectline/content.

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

#### 2.Slope(m)=(y2-y1)/(x2-x1)
#### 3.Intercept= b


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

