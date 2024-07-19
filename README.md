# Logistic Regression Implementation

## Overview
This project involves implementing multivariate logistic regression and learning its solution using Stochastic Gradient Descent (SGD). The goal is to perform binary classification and compare the logistic regression model's performance with a random classifier.

## Dataset
The dataset used is `Weekly`, which contains weekly percentage returns for the S&P 500 stock index between 1990 and 2010. This dataset contains 1089 observations on the following 9 features:
- **Year**: The year that the observation was recorded.
- **Lag1**: Percentage return for the previous week.
- **Lag2**: Percentage return for 2 weeks previous.
- **Lag3**: Percentage return for 3 weeks previous.
- **Lag4**: Percentage return for 4 weeks previous.
- **Lag5**: Percentage return for 5 weeks previous.
- **Volume**: Volume of shares traded (average number of daily shares traded in billions).
- **Today**: Percentage return for this week.

The output variable is **Direction**, a factor with levels "Down" and "Up" indicating whether the market had a positive or negative return on a given week.

## Project Steps
1. **Data Preparation**:
   - Load the dataset and prepare the features and labels for logistic regression.
   - Add a column of ones to the features matrix to create the bias term.

2. **Mini-Batch Stochastic Gradient Descent**:
   - Implement a mini-batch stochastic gradient descent approach to logistic regression.
   - Use a decreasing stepsize to satisfy Robbins-Monro convergence.
   - Set the number of epochs to 200.
   - Compare the speed of convergence with the Momentum method.
   - Report the errors.

3. **Comparison with k-NN Classifiers**:
   - Compare the logistic regression results with k-NN classifiers for k = 3, 5, 7.
   - Evaluate the performance based on accuracy and error rates.

## Requirements
- Python 3.x
- Libraries: pandas, numpy, scikit-learn

## How to Run
1. Clone the repository.
2. Install the required libraries.
3. Run the `LogReg.py` script to execute the logistic regression model.

## Results
- Errors and convergence speeds for the mini-batch SGD logistic regression.
- Comparison of logistic regression performance with k-NN classifiers.

## Conclusion
This project demonstrates the implementation of logistic regression using SGD and compares its performance with k-NN classifiers. The logistic regression model is expected to outperform a random classifier.


