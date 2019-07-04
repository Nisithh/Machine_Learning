# Machine_Learning
Machine Learning 

Types of Machine Learning:
1.Regression
2.Classification
3.Clustering

1. Regression:- Output variable predicted on the basis of past data over continuous/numeric dataset resulted to a continuous variable.
                for example- creating merit list for qualified students for Post graduation Programs on the basis of graduation score.
2. Classification:- Output variable predicted on the basis of past data over categorical/label dataset resulted to a categorical variable.
                    for example:-Classifying emails on the basis of subjectline/content.
3. Clustering:-  Output Variable predicted on the basis of large amount of data over without labeled dataset resulted to a categorical                      variable after analysis for example- customer segmentation on the large amount of customer dataset

*----Point To be Noted---*
1.Regression and Classification Comes under Supervised Learning
2.In both of them we have Labels
3.Regression has Continuous/numeric labels  in dataset
4.Classification has Categorical Labels in dataset
5.Both gives result on the basis of Past behaviour of dataset.

*----Point to be Noted---*
1.Clustering Comes under Un-Supervised Learning
2.it doesn't have labels and here we have large amount of dataset 
3.Result comes as a categorical variable after analysis.

*----Point to be Noted---*
Predictive analysis is used to build the model on training data and the we predict on the test data if our model has passed the tests.


Linear Regression Line:-

1.The equation of a straight line is usually written this way:
y = mx + b

2.
![Capture1](https://user-images.githubusercontent.com/16449922/60673158-c2ad5a80-9e94-11e9-9e1e-f991ef37c201.JPG)

3.Slope(m)=(y2-y1)/(x2-x1)
4.Intercept= b


5.Machine Learning Standard Notation for Straight line:
y=β0+β1x

6.For fitting the best line in Scatter Plot
We find out Residuals

Residual(ei)=yi-ypred

here ei is the error at a particlar datapoint
yi is the actual value at that data point
ypred is the predicted value at a particular datapoint

To minimize the error here we use ordinary least squares method
RSS(Residual Sum Of Squares)=sqrt(e1)+sqrt(e2)+---+sqrt(en)

--Now when we replace value of  Yi & Ypred
RSS=Sqrt(y1-β0-β1x1)+Sqrt(y2-β0-β1x2)+----+Sqrt(yn-β0-β1xn)

![Capture2](https://user-images.githubusercontent.com/16449922/60679612-dca36900-9ea5-11e9-94f9-3823f085f02e.JPG)



