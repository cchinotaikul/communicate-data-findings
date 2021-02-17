# Data Exploration - Loan Data from Prosper
## by Chinnaporn Chinotaikul


## Dataset

This document explores a dataset of loans taken on Prosper, a peer-to-peer lending platform. The data set consists of 113,937 loans at Prosper from 2005 to 2014, with each row representing 1 loan. There are 81 variables.

## Summary of Findings

- Loan outcome (successful completion or fail-to-collect) appears to have the strongest correlation with Prosper Rating
- Prosper Rating is a proprietary measure of credit which appears to incorporate credit scoring inputs (including the borrower's credit history) and other factors such as the borrower's employment
- Loan outcomes also appear to correlate with other factors such as loan term, size and recommendations from other Prosper users

## Key Insights for Presentation

- Univariate exploration for loan outcome and Prosper Rating distributions are shown in the presentation. The distribution for loan size (divided by loan term month) is also shown to support the multivariate section
  - Approx. 78% of loans are successfully completed
  - Prosper Rating ranges from 1 to 7 with 7 being the best. The most common rating is 3 while the least common is 7. The other values have approximately the same amounts.

- Bivariate exploration:
  - Plotting outcome vs Prosper Rating shows that completed loans do tend to have higher average rating compared to loans that failed to collect

- Multivariate exploration
  - The terms of loans in the dataset consist only of 12-, 36- and 60-months. By plotting outcome vs rating and separating the charts by terms, some interesting observations can be made, including that the stongest correlation between Rating and outcome can be seen in 38-month loans while the weakest correlation is at 60-month loans
  - When separating by loan size, it can be seen that the rating to outcome relationship holds at most loan sizes
  - Each borrower can have recommendations by other Prosper users. The vast majority of users have 0 recommendations. Some have 1-2 recommendations but 3 and above are very rare. If a borrower has at least one recommendation, the expected outcome of the loan improves significantly

## Resources used
- Udacity course materials
- Numpy, Pandas, Matplotlib and Seaborn documentations
- Code for adjusting labels for scatter matrix taken from https://stackoverflow.com/questions/58623528/pandas-scatter-matrix-labels-vertical-x-and-horizontal-y-without-being-cut
