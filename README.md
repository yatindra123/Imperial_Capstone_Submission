# PROJECT TITLE 
Predicting Salaries of Baseball Players (using Hitters Dataset from ISLR Library)

Please see full report in the following attached Word document: Capstone Project Report February 19 2024


## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
The goal of the project is to predict the salaries of Baseball players using the dataset “Hitters” which is Major League Baseball Data from the 1986 and 1987 seasons. The data is available as a dataframe with 322 observations and 20 columns. This includes the “Salary” column that we would like to predict using the remaining variables as predictors. We built six different regression models on the training data, using them to predict for the test data and calculate their accuracy relative to the actual salary using metrics like MSE and R^2 after optimizing their key hyperparameters. The various techniques used are as follows:

A.	Single Decision Tree
B.	Random Forest 
C.	Boosting
D.	Linear Regression
E.	Ridge Regression
F.	Lasso


## DATA
The data is referenced in the book “Introduction to Statistical Learning (ISLR)” by James, Witten, Hastie and Tibshirani and downloaded from the website https://rdrr.io/cran/ISLR/man/Hitters.html.

This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University. This is part of the data that was used in the 1988 ASA Graphics Section Poster Session. The salary data were originally from Sports Illustrated, April 20, 1987. The 1986 and career statistics were obtained from The 1987 Baseball Encyclopedia Update published by Collier Books, Macmillan Publishing Company, New York (source: above referenced website).


## MODEL 
We randomly split the data into 50% training data (131 rows), 25% validation data (65 rows) and 25% testing data (67 rows).

We now build six different regression models on the training data, using them to predict for the test data and calculate their accuracy relative to the actual salary using metrics like MSE and R^2.

A.	Single Decision Tree (Hyperparameter optimized: Tree depth)
B.	Random Forest (Hyperparameter optimized: Maximum number of parameters selected)
C.	Boosting 
D.	Linear Regression
E.	Ridge Regression (Hyperparameter optimized: Tuning Parameter)
F.	Lasso (Hyperparameter optimized: Tuning Parameter)


## HYPERPARAMETER OPTIMSATION

A.	Single Decision Tree (Hyperparameter optimized: Tree depth)
B.	Random Forest (Hyperparameter optimized: Maximum number of parameters selected)
C.	Boosting 
D.	Linear Regression
E.	Ridge Regression (Hyperparameter optimized: Tuning Parameter)
F.	Lasso (Hyperparameter optimized: Tuning Parameter)

Grid optimization was used.

## RESULTS
The Random Forest regression model for the tuned hyperparameter had the best performance among all the predictive models that were attempted. The R^2 values are as follows:

Decision Tree Regression:
Validation Score: 0.5587164537125167
Test Score: 0.7070098247833088

Random Forest Regression:
Validation Score: 0.6595974698501812
Test Score: 0.8712581992377905

AdaBoost Regression:
Validation Score: 0.6450184594199913
Test Score: 0.8445658526697923

Linear Regression:
Training Score: 0.464
Validation Score: 0.442
Test Score: 0.607

Lasso Regression:
Training Score: 0.39542608940321855
Validation Score: 0.4463604614947928
Test Score: 0.5539347145646234

Ridge Regression:
Training Score: 0.4644679866586633
Validation Score: 0.4417290978326277
Test Score: 0.606398624139123

The decision tree regression models with tuned hyperparameters are doing better as a group compared to the variants of linear regression models that were attempted. This is also evident in the below line chart comparing predicted Salary (log transform values) to actuals values for the various regression models.


You can include images of plots using the code below: 
Detailed charts and results are available in the full project report attached with the submission: Capstone Project Report February 19 2024 (Word document)
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

The full Jupyter notebook is attached with the project submission:
Capstone Project Decision Tree and Linear Regression on Hitters Data February 2024.ipynb

