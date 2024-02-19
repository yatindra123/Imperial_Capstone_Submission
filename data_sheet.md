# Datasheet Template

As far as you can, complete the model datasheet. If you have got the data from the internet, you may not have all the information you need, but make sure you include all the information you do have. 

## Motivation

- For what purpose was the dataset created? 
- Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?

The dataset “Hitters” contains Major League Baseball Data from the 1986 and 1987 seasons. The data is referenced in the book “Introduction to Statistical Learning (ISLR)” by James, Witten, Hastie and Tibshirani and downloaded from the website https://rdrr.io/cran/ISLR/man/Hitters.html.

This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University. This is part of the data that was used in the 1988 ASA Graphics Section Poster Session. The salary data were originally from Sports Illustrated, April 20, 1987. The 1986 and career statistics were obtained from The 1987 Baseball Encyclopedia Update published by Collier Books, Macmillan Publishing Company, New York (source: above referenced website).

 
## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? 
- How many instances of each type are there? 
- Is there any missing data?
- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?


The data is available as a dataframe with 322 observations and 20 columns. This includes the “Salary” column that we would like to predict using the remaining variables as predictors. Salary is missing for 59 records. The data is not confidential.

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
 

## Collection process

- How was the data acquired? 
- If the data is a sample of a larger subset, what was the sampling strategy? 
- Over what time frame was the data collected?

This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University. This is part of the data that was used in the 1988 ASA Graphics Section Poster Session. The salary data were originally from Sports Illustrated, April 20, 1987. The 1986 and career statistics were obtained from The 1987 Baseball Encyclopedia Update published by Collier Books, Macmillan Publishing Company, New York (source: above referenced website).

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section. 
- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? 
 
## Uses

- What other tasks could the dataset be used for? 
- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms? 
- Are there tasks for which the dataset should not be used? If so, please provide a description.

There are no restrictions to the use of this data. However, it is fairly dated and so salary predictions and the predictor variables are likely to have changed in the 35+ years since the data was created.

## Distribution

- How has the dataset already been distributed? 
- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)? 

No copyright restrictions. This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University. This is part of the data that was used in the 1988 ASA Graphics Section Poster Session. The salary data were originally from Sports Illustrated, April 20, 1987. The 1986 and career statistics were obtained from The 1987 Baseball Encyclopedia Update published by Collier Books, Macmillan Publishing Company, New York (source: above referenced website).

## Maintenance

- Who maintains the dataset?

This dataset was taken from the StatLib library which is maintained at Carnegie Mellon University. 

