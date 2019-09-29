# Machine_Learning Models
Types of Machine Learning models:

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

## Simple linear regression

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

#### Conclusion:-

It is clear that no line can be found to pass through all points of the plot. Thus no functional relation exists between the two variables x and Y. However, the scatter plot does give an indication that a straight line may exist such that all the points on the plot are scattered randomly around this line. A statistical relation is said to exist in this case. The statistical relation between x and Y  may be expressed as follows:

![Capture2](https://user-images.githubusercontent.com/16449922/60742000-2a44d200-9f89-11e9-8df8-8523a89cf76f.JPG)

The above equation is the linear regression model that can be used to explain the relation between x and Y  that is seen on the scatter plot above. In this model, the mean value of Y (abbreviated as E(Y) ) is assumed to follow the linear relation:

![Capture3](https://user-images.githubusercontent.com/16449922/60742028-421c5600-9f89-11e9-8c5d-9a3fea53aebc.JPG)


The actual values of  (which are observed as yield from the chemical process from time to time and are random in nature) are assumed to be the sum of the mean value,E(Y) , and a random error term epsilon :

![Capture1](https://user-images.githubusercontent.com/16449922/60741915-ece04480-9f88-11e9-9b36-bbe10b505245.JPG)

The regression model here is called a simple linear regression model because there is just one independent variable x , in the model. In regression models, the independent variables are also referred to as regressors or predictor variables. The dependent variable Y  , is also referred to as the response. The slope,β1 , and the intercept,β0  , of the line E(Y) are called regression coefficients. The slope,β1 , can be interpreted as the change in the mean value of Y  for a unit change in x.

The random error term,epsilon , is assumed to follow the normal distribution with a mean of 0 and variance of ![Capture4](https://user-images.githubusercontent.com/16449922/60742306-7cd2be00-9f8a-11e9-920d-5fd11fe8d12d.JPG)
. Since  is the sum of this random term and the mean value,E(Y) , which is a constant, the variance of Y at any given value of x  is also ![Capture4](https://user-images.githubusercontent.com/16449922/60742306-7cd2be00-9f8a-11e9-920d-5fd11fe8d12d.JPG)
. Therefore, at any given value of x, say xi , the dependent variable Y follows a normal distribution with a mean of β0+β1xi and a standard deviation of ![Capture4](https://user-images.githubusercontent.com/16449922/60742306-7cd2be00-9f8a-11e9-920d-5fd11fe8d12d.JPG)  . This is illustrated in the following figure.

![Capture2](https://user-images.githubusercontent.com/16449922/60738546-53ab3100-9f7c-11e9-8c8d-a24ec185236b.JPG)

Now 
 
![Capture1](https://user-images.githubusercontent.com/16449922/60738619-9836cc80-9f7c-11e9-9563-a1bfd75d8979.JPG)

where β0 & β1 with a hat notion represents that these are estimated values

#### now is this sufficient for inference?-No
again now let's find out what does simple linear regression do:-

![Capture2](https://user-images.githubusercontent.com/16449922/60739248-ddf49480-9f7e-11e9-8ae9-a983d105d25f.JPG)

#### Looking at the graph statistically

![Capture3](https://user-images.githubusercontent.com/16449922/60739336-27dd7a80-9f7f-11e9-8192-c379ac569128.JPG)

![Capture1](https://user-images.githubusercontent.com/16449922/60739379-58251900-9f7f-11e9-8206-3c3262dd4536.JPG)

Let's understand the importance of each assumption one by one:
 
#### There is a linear relationship between X and Y:

X and Y should display some sort of a linear relationship; otherwise, there is no use of fitting a linear model between them

![Capture1](https://user-images.githubusercontent.com/16449922/60740383-19915d80-9f83-11e9-98ed-d899f5dc5c37.JPG)

#### Violations of linearity or additivity are extremely serious: 
if you fit a linear model to data which are nonlinearly or nonadditively related, your predictions are likely to be seriously in error, especially when you extrapolate beyond the range of the sample data.

#### How to diagnose: 
nonlinearity is usually most evident in a plot of observed versus predicted values or a plot of residuals versus predicted values, which are a part of standard regression output. The points should be symmetrically distributed around a diagonal line in the former plot or around horizontal line in the latter plot, with a roughly constant variance.  (The residual-versus-predicted-plot is better than the observed-versus-predicted plot for this purpose, because it eliminates the visual distraction of a sloping pattern.)  Look carefully for evidence of a "bowed" pattern, indicating that the model makes systematic errors whenever it is making unusually large or small predictions. In multiple regression models, nonlinearity or nonadditivity may also be revealed by systematic patterns in plots of the residuals versus individual independent variables.

#### How to fix: 
if the data are strictly positive, the log transformation is an option.  (The logarithm base does not matter--all log functions are same up to linear scaling--although the natural log is usually preferred because small changes in the natural log are equivalent to percentage changes.  See these notes for more details.)  If a log transformation is applied to the dependent variable only, this is equivalent to assuming that it grows (or decays) exponentially as a function of the independent variables.  If a log transformation is applied to both the dependent variable and the independent variables, this is equivalent to assuming that the effects of the independent variables are multiplicative rather than additive in their original units. This means that, on the margin, a small percentage change in one of the independent variables induces a proportional percentage change in the expected value of the dependent variable, other things being equal.

Another possibility to consider is adding another regressor that is a nonlinear function of one of the other variables. For example, if you have regressed Y on X, and the graph of residuals versus predicted values suggests a parabolic curve, then it may make sense to regress Y on both X and X^2 (i.e., X-squared). The latter transformation is possible even when X and/or Y have negative values, whereas logging is not. 

you need to beware of overfitting the sample data by throwing in artificially constructed variables that are poorly motivated.

#### Error terms are normally distributed with mean zero(not X, Y):

1.There is no problem if the error terms are not normally distributed if you just wish to fit a line and not make any further interpretations.
2.But if you are willing to make some inferences on the model that you have built , you need to have a notion of the distribution of the error terms. One particular repercussion of the error terms not being normally distributed is that the p-values obtained during the hypothesis test to determine the significance of the coefficients become unreliable.
3.The assumption of normality is made, as it has been observed that the error terms generally follow a normal distribution with mean equal to zero in most cases.

![Capture2](https://user-images.githubusercontent.com/16449922/60740460-72f98c80-9f83-11e9-8cf0-f35c0d35e455.JPG)


#### Violations of normality 
create problems for determining whether model coefficients are significantly different from zero and for calculating confidence intervals for forecasts. Sometimes the error distribution is "skewed" by the presence of a few large outliers. Since parameter estimation is based on the minimization of squared error, a few extreme observations can exert a disproportionate influence on parameter estimates. Calculation of confidence intervals and various significance tests for coefficients are all based on the assumptions of normally distributed errors. If the error distribution is significantly non-normal, confidence intervals may be too wide or too narrow.

Technically, the normal distribution assumption is not necessary if you are willing to assume the model equation is correct and your only goal is to estimate its coefficients and generate predictions in such a way as to minimize mean squared error.  The formulas for estimating coefficients require no more than that, and some references on regression analysis do not list normally distributed errors among the key assumptions.  But generally we are interested in making inferences about the model and/or estimating the probability that a given forecast error will exceed some threshold in a particular direction, in which case distributional assumptions are important.  Also, a significant violation of the normal distribution assumption is often a "red flag" indicating that there is some other problem with the model assumptions and/or that there are a few unusual data points that should be studied closely and/or that a better model is still waiting out there somewhere.

#### How to diagnose: 
the best test for normally distributed errors is a normal probability plot or normal quantile plot of the residuals. These are plots of the fractiles of error distribution versus the fractiles of a normal distribution having the same mean and variance. If the distribution is normal, the points on such a plot should fall close to the diagonal reference line. A bow-shaped pattern of deviations from the diagonal indicates that the residuals have excessive skewness (i.e., they are not symmetrically distributed, with too many large errors in one direction). An S-shaped pattern of deviations indicates that the residuals have excessive kurtosis--i.e., there are either too many or two few large errors in both directions.  Sometimes the problem is revealed to be that there are a few data points on one or both ends that deviate significantly from the reference line ("outliers"), in which case they should get close attention. 

There are also a variety of statistical tests for normality, including the Kolmogorov-Smirnov test, the Shapiro-Wilk test, the Jarque-Bera test, and the Anderson-Darling test.  The Anderson-Darling test (which is the one used by RegressIt) is generally considered to be the best, because it is specific to the normal distribution (unlike the K-S test) and it looks at the whole distribution rather than just the skewness and kurtosis (like the J-B test).  But all of these tests are excessively "picky" in this author’s opinion.  Real data rarely has errors that are perfectly normally distributed, and it may not be possible to fit your data with a model whose errors do not violate the normality assumption at the 0.05 level of significance.  It is usually better to focus more on violations of the other assumptions and/or the influence of a few outliers (which may be mainly responsible for violations of normality anyway) and to look at a normal probability plot or normal quantile plot and draw your own conclusions about whether the problem is serious and whether it is systematic.

Here is an example of a bad-looking normal quantile plot (an S-shaped pattern with P=0 for the A-D stat, indicating highly significant non-normality)

![Capture1](https://user-images.githubusercontent.com/16449922/60741613-c1a92580-9f87-11e9-9dbe-4725c7c4ffe5.JPG)

and here is an example of a good-looking one (a linear pattern with P=0.5 for the A-D stat, indicating no significant departure from normality):

![Capture2](https://user-images.githubusercontent.com/16449922/60741671-f5844b00-9f87-11e9-875e-299d1104c2e4.JPG)



#### How to fix:
violations of normality often arise either because (a) the distributions of the dependent and/or independent variables are themselves significantly non-normal, and/or (b) the linearity assumption is violated. In such cases, a nonlinear transformation of variables might cure both problems. In the case of the two normal quantile plots above, the second model was obtained applying a natural log transformation to the variables in the first one. 

The dependent and independent variables in a regression model do not need to be normally distributed by themselves--only the prediction errors need to be normally distributed.  (In fact, independent variables do not even need to be random, as in the case of trend or dummy or treatment or pricing variables.)  But if the distributions of some of the variables that are random are extremely asymmetric or long-tailed, it may be hard to fit them into a linear model whose errors will be normally distributed, and explaining the shape of their distributions may be an interesting topic all by itself.  Keep in mind that the normal error assumption is usually justified by appeal to the central limit theorem, which holds in the case where many random variations are added together.  If the underlying sources of randomness are not interacting additively, this argument fails to hold.

Another possibility is that there are two or more subsets of the data having different statistical properties, in which case separate models should be built, or else some data should merely be excluded, provided that there is some a priori criterion that can be applied to make this determination.

In some cases, the problem with the error distribution is mainly due to one or two very large errors. Such values should be scrutinized closely: are they genuine (i.e., not the result of data entry errors), are they explainable, are similar events likely to occur again in the future, and how influential are they in your model-fitting results? If they are merely errors or if they can be explained as unique events not likely to be repeated, then you may have cause to remove them. In some cases, however, it may be that the extreme values in the data provide the most useful information about values of some of the coefficients and/or provide the most realistic guide to the magnitudes of forecast errors.


#### Error terms are independent of each other:

The error terms should not be dependent on one another (like in a time-series data wherein the next value is dependent on the previous one).

![Capture3](https://user-images.githubusercontent.com/16449922/60740544-c23fbd00-9f83-11e9-9270-4c4275f716b8.JPG)


#### Violations of independence are potentially very serious in time series regression models: 
serial correlation in the errors (i.e., correlation between consecutive errors or errors separated by some other number of periods) means that there is room for improvement in the model, and extreme serial correlation is often a symptom of a badly mis-specified model. Serial correlation (also known as autocorrelation”) is sometimes a byproduct of a violation of the linearity assumption, as in the case of a simple (i.e., straight) trend line fitted to data which are growing exponentially over time. 

Independence can also be violated in non-time-series models if errors tend to always have the same sign under particular conditions, i.e., if the model systematically underpredicts or overpredicts what will happen when the independent variables have a particular configuration. 

#### How to diagnose: 
The best test for serial correlation is to look at a residual time series plot (residuals vs. row number) and a table or plot of residual autocorrelations. (If your software does not provide these by default for time series data, you should figure out where in the menu or code to find them.) Ideally, most of the residual autocorrelations should fall within the 95% confidence bands around zero, which are located at roughly plus-or-minus 2-over-the-square-root-of-n, where n is the sample size. Thus, if the sample size is 50, the autocorrelations should be between +/- 0.3. If the sample size is 100, they should be between +/- 0.2. Pay especially close attention to significant correlations at the first couple of lags and in the vicinity of the seasonal period, because these are probably not due to mere chance and are also fixable. The Durbin-Watson statistic provides a test for significant residual autocorrelation at lag 1: the DW stat is approximately equal to 2(1-a) where a is the lag-1 residual autocorrelation, so ideally it should be close to 2.0--say, between 1.4 and 2.6 for a sample size of 50.

#### How to fix: 
Minor cases of positive serial correlation (say, lag-1 residual autocorrelation in the range 0.2 to 0.4, or a Durbin-Watson statistic between 1.2 and 1.6) indicate that there is some room for fine-tuning in the model. Consider adding lags of the dependent variable and/or lags of some of the independent variables. Or, if you have an ARIMA+regressor procedure available in your statistical software, try adding an AR(1) or MA(1) term to the regression model.  An AR(1) term adds a lag of the dependent variable to the forecasting equation, whereas an MA(1) term adds a lag of the forecast error. If there is significant correlation at lag 2, then a 2nd-order lag may be appropriate.

If there is significant negative correlation in the residuals (lag-1 autocorrelation more negative than -0.3 or DW stat greater than 2.6), watch out for the possibility that you may have overdifferenced some of your variables. Differencing tends to drive autocorrelations in the negative direction, and too much differencing may lead to artificial patterns of negative correlation that lagged variables cannot correct for.

If there is significant correlation at the seasonal period (e.g. at lag 4 for quarterly data or lag 12 for monthly data), this indicates that seasonality has not been properly accounted for in the model. Seasonality can be handled in a regression model in one of the following ways: (i) seasonally adjust the variables (if they are not already seasonally adjusted), or (ii) use seasonal lags and/or seasonally differenced variables (caution: be careful not to overdifference!), or (iii) add seasonal dummy variables to the model (i.e., indicator variables for different seasons of the year, such as MONTH=1 or QUARTER=2, etc.) The dummy-variable approach enables additive seasonal adjustment to be performed as part of the regression model: a different additive constant can be estimated for each season of the year. If the dependent variable has been logged, the seasonal adjustment is multiplicative. (Something else to watch out for: it is possible that although your dependent variable is already seasonally adjusted, some of your independent variables may not be, causing their seasonal patterns to leak into the forecasts.)

Major cases of serial correlation (a Durbin-Watson statistic well below 1.0, autocorrelations well above 0.5) usually indicate a fundamental structural problem in the model. You may wish to reconsider the transformations (if any) that have been applied to the dependent and independent variables. It may help to stationarize all variables through appropriate combinations of differencing, logging, and/or deflating.

To test for non-time-series violations of independence, you can look at plots of the residuals versus independent variables or plots of residuals versus row number in situations where the rows have been sorted or grouped in some way that depends (only) on the values of the independent variables.  The residuals should be randomly and symmetrically distributed around zero under all conditions, and in particular there should be no correlation between consecutive errors no matter how the rows are sorted, as long as it is on some criterion that does not involve the dependent variable.  If this is not true, it could be due to a violation of the linearity assumption or due to bias that is explainable by omitted variables (say, interaction terms or dummies for identifiable conditions).

#### Error terms have constant variance (homoscedasticity):

The variance should not increase (or decrease) as the error values change,Also, the variance should not follow any pattern as the error terms change.

![Capture4](https://user-images.githubusercontent.com/16449922/60740636-1f3b7300-9f84-11e9-816d-6c82753490de.JPG)

#### Violations of homoscedasticity 
(which are called "heteroscedasticity") make it difficult to gauge the true standard deviation of the forecast errors, usually resulting in confidence intervals that are too wide or too narrow. In particular, if the variance of the errors is increasing over time, confidence intervals for out-of-sample predictions will tend to be unrealistically narrow. Heteroscedasticity may also have the effect of giving too much weight to a small subset of the data (namely the subset where the error variance was largest) when estimating coefficients.

#### How to diagnose: 
look at a plot of residuals versus predicted values and, in the case of time series data, a plot of residuals versus time.  Be alert for evidence of residuals that grow larger either as a function of time or as a function of the predicted value. To be really thorough, you should also generate plots of residuals versus independent variables to look for consistency there as well.  Because of imprecision in the coefficient estimates, the errors may tend to be slightly larger for forecasts associated with predictions or values of independent variables that are extreme in both directions, although the effect should not be too dramatic.  What you hope not to see are errors that systematically get larger in one direction by a significant amount.

#### How to fix:  
If the dependent variable is strictly positive and if the residual-versus-predicted plot shows that the size of the errors is proportional to the size of the predictions (i.e., if the errors seem consistent in percentage rather than absolute terms), a log transformation applied to the dependent variable may be appropriate.  In time series models, heteroscedasticity often arises due to the effects of inflation and/or real compound growth. Some combination of logging and/or deflating will often stabilize the variance in this case. Stock market data may show periods of increased or decreased volatility over time. This is normal and is often modeled with so-called ARCH (auto-regressive conditional heteroscedasticity) models in which the error variance is fitted by an autoregressive model. Such models are beyond the scope of this discussion, but a simple fix would be to work with shorter intervals of data in which volatility is more nearly constant. Heteroscedasticity can also be a byproduct of a significant violation of the linearity and/or independence assumptions, in which case it may also be fixed as a byproduct of fixing those problem. 

Seasonal patterns in the data are a common source of heteroscedasticity in the errors:  unexplained variations in the dependent variable throughout the course of a season may be consistent in percentage rather than absolute terms, in which case larger errors will be made in seasons where activity is greater, which will show up as a seasonal pattern of changing variance on the residual-vs-time plot.  A log transformation is often used to address this problem.  For example, if the seasonal pattern is being modeled through the use of dummy variables for months or quarters of the year, a log transformation applied to the dependent variable will convert the coefficients of the dummy variables to multiplicative adjustment factors rather than additive adjustment factors, and the errors in predicting the logged variable will be (roughly) interpretable as percentage errors in predicting the original variable.  Seasonal adjustment of all the data prior to fitting the regression model might be another option. 

If a log transformation has already been applied to a variable, then (as noted above) additive rather than multiplicative seasonal adjustment should be used, if it is an option that your software offers.  Additive seasonal adjustment is similar in principle to including dummy variables for seasons of the year.  Whether-or-not you should perform the adjustment outside the model rather than with dummies depends on whether you want to be able to study the seasonally adjusted data all by itself and on whether there are unadjusted seasonal patterns in some of the independent variables.  (The dummy-variable approach would address the latter problem.) 


###### Hypothesis Testing in Linear Regression

every time you perform a linear regression, you need to test whether the fitted line is a significant one or not or to simply put it, you need to test whether β1 is significant or not

For that purpose we use Hypotheses testing in Linear Regresion-

So if β1  is not significant, i.e. there is no relationship between X and y.

So in order to perform the hypothesis test, we first propose the null hypothesis that 
β1 is 0. And the alternative hypothesis thus becomes 
β1 is not zero.

### Null Hypothesis (H0): β1=0
### Alternate Hypothesis (HA):β1≠0

So this hypothesis test will be- 
If you fail to reject the null hypothesis that would mean that β1 is zero which would simply mean that β1 is insignificant and of no use in the model. 

Similarly, if you reject the null hypothesis, it would mean that β1 is not zero and the line fitted is a significant one.

first compute the t-score (which is very similar to the Z-score) which is given by 

(X−μ)/(s/√n)

where μ is the population mean and s is the sample standard deviation which when divided by √n is also known as standard error.

Using this, the t-score for estimated β1 comes out to be (since the null hypothesis is that 
β1 is equal to zero):

(β1−0)/SE(β1) --------here β1 is estimated β1

Now, in order to perform the hypothesis test, you need to derive the p-value for the given beta.

Let's do a quick recap of how do you calculate p-value:

Calculate the value of t-score for the mean point (in this case, zero, according to the Null hypothesis that we have stated) on the distribution
Calculate the p-value from the cumulative probability for the given t-score using the t-table
Make the decision on the basis of the p-value with respect to the given value of β  (significance level)

Now, if the p-value turns out to be less than 0.05, you can reject the null hypothesis and state that β1 is indeed significant.


## Multiple Linear Regression

### Equation: Y=β0+β1X1+β2X2+...+βpXp+ϵ

![Capture1](https://user-images.githubusercontent.com/16449922/60757339-e0122e00-a026-11e9-84d6-f4e9eb682d11.JPG)


![Capture2](https://user-images.githubusercontent.com/16449922/60757479-f8834800-a028-11e9-944f-9c6ae232b688.JPG)

### Multicollinearity

![Capture3](https://user-images.githubusercontent.com/16449922/60758040-e35de780-a02f-11e9-86c5-864c87a540de.JPG)

![Capture4](https://user-images.githubusercontent.com/16449922/60758193-07bac380-a032-11e9-8592-06d908dfa330.JPG)

The common heuristic we follow for the VIF values is:

> 10:  Definitely high VIF value and the variable should be eliminated.

> 5:  Can be okay, but it is worth inspecting.

< 5: Good VIF value. No need to eliminate this variable.


Some methods that can be used to deal with multicollinearity are:

#### 1.Dropping variables

Drop the variable which is highly correlated with others

Pick the business interpretable variable

#### 2.Create new variable using the interactions of the older variables

Add interaction features, i.e. features derived using some of the original features

#### 3.Variable transformations

Principal Component Analysis 


#### Scaling:-

It is important to note that scaling just affects the coefficients and none of the other parameters like t-statistic, F-statistic, p-values, R-squared, etc.

There are two major methods to scale the variables, i.e. standardisation and MinMax scaling. Standardisation basically brings all of the data into a standard normal distribution with mean zero and standard deviation one. MinMax scaling, on the other hand, brings all of the data in the range of 0 and 1. The formulae in the background used for each of these methods are as given below: 

Standardisation:  x=(x−mean(x))/sd(x)

MinMax Scaling: x=(x−min(x))/(max(x)−min(x))


![Capture1](https://user-images.githubusercontent.com/16449922/60758932-c11d9700-a03a-11e9-968e-2cfdd05f913f.JPG)


![Capture2](https://user-images.githubusercontent.com/16449922/60758943-e5797380-a03a-11e9-81ab-ba64d9e5d33d.JPG)

#### *---Point to be noted---*
Adjusted R-squared on the other hand, penalises models based on the number of variables present in it. So if you add a variable and the Adjusted R-squared drops, you can be certain that that variable is insignificant to the model and shouldn't be used. So in the case of multiple linear regression, you should always look at the adjusted R-squared value in order to keep redundant variables out from your regression model.

#### Feature Selection

Try all possible combinations--
2^p models for p features

To get the optimal model, 
you can always try all the possible combinations of independent variables and see which model fits the best. But this method is obviously, time-consuming and infeasible. Hence, you need some other method to get a decent model. This is where manual feature elimination comes in, where you:


Build the model with all the features
Drop the features that are least helpful in prediction (high p-value)
Drop the features that are redundant (using correlations and VIF)
Rebuild model and repeat

![Capture3](https://user-images.githubusercontent.com/16449922/60759252-ae599100-a03f-11e9-8e7c-de330f7ab935.JPG)

another reasonable approach is -
Comination-
first use automated coarse tuning
then use manula fine tuning


#### RFE

the coefficients of a linear model), the goal of recursive feature elimination (RFE) is to select features by recursively considering smaller and smaller sets of features. First, the estimator is trained on the initial set of features and the importance of each feature is obtained either through a coef_ attribute or through a feature_importances_ attribute. Then, the least important features are pruned from current set of features. That procedure is recursively repeated on the pruned set until the desired number of features to select is eventually reached.

#### *---Point to be noted---*
A high p-value means that the variable is not significant, and hence, doesn't help much in prediction.




