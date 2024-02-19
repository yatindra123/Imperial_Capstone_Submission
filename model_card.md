# Model Card

See the [example Google model cards](https://modelcards.withgoogle.com/model-reports) for inspiration. 

Detailed charts and results are available in the full project report attached with the submission: Capstone Project Report February 19 2024 (Word document)

## Model Description

**Input:** Describe the inputs of your model 

**Output:** Describe the output(s) of your model

**Model Architecture:** Describe the model architecture you’ve used

The data is available as a dataframe with 322 observations and 20 columns. This includes the “Salary” column that we would like to predict using the remaining variables as predictors.

AtBat
Number of times at bat in 1986
Hits
Number of hits in 1986
HmRun
Number of home runs in 1986
Runs
Number of runs in 1986
RBI
Number of runs batted in in 1986
Walks
Number of walks in 1986
Years
Number of years in the major leagues
CAtBat
Number of times at bat during his career
CHits
Number of hits during his career
CHmRun
Number of home runs during his career
CRuns
Number of runs during his career
CRBI
Number of runs batted in during his career
CWalks
Number of walks during his career
League
A factor with levels A and N indicating player's league at the end of 1986
Division
A factor with levels E and W indicating player's division at the end of 1986
PutOuts
Number of put outs in 1986
Assists
Number of assists in 1986
Errors
Number of errors in 1986
Salary
1987 annual salary on opening day in thousands of dollars
NewLeague
A factor with levels A and N indicating player's league at the beginning of 1987

Variables like League, Division and NewLeague are categorical and are converted into numerical variables for further analysis. Also, all 59 rows with missing Salary values are removed. This leads to a new dataset with 263 rows and 23 columns. Excluding the predicted variable (Salary) and the categorical variables (League, Division and NewLeague), there are 19 numerical predictor variables.

A detailed model exploration was conducted including summary statistics and bivariate charts exploring the relationship between Salary and the 19 predictor variables. Detailed charts and results are available in the full project report attached with the submission: Capstone Project Report February 19 2024 (Word document)

We now randomly split the data into 50% training data (131 rows), 25% validation data (65 rows) and 25% testing data (67 rows).

We now build six different regression models on the training data, using them to predict for the test data and calculate their accuracy relative to the actual salary using metrics like MSE and R^2.

A.	Single Decision Tree
B.	Random Forest 
C.	Boosting
D.	Linear Regression
E.	Ridge Regression
F.	Lasso


## Performance

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

Detailed charts and results are available in the full project report attached with the submission: Capstone Project Report February 19 2024 (Word document)


## Limitations

Given more sample and time, I would have attempted to further fine tune the hyperparameters using k-fold cross-validation. I would also want to tune some of the other hyperparameters. I am surprised that the tuning parameter in Ridge Regression and Lasso did not produce more appreciable sloping of outcomes and suspect that this was because I did not cover a fuller range of possibilities. Finally, I noticed that even the best of the above regression models – Random Forest – underpredicts at the upper end of the Salary range and overpredicts at the lower end of the Salary range. I wonder if this is because an important predictor variable is missing from the available list. It could also be because all the hyperparameters are not sufficiently tuned.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
