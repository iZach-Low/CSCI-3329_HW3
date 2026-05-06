# CSCI 3329 - Homework 3 Report
## 1. Dataset
- Student Performance Dataset (UCI)
- 649 Samples with 30 features
- 3 classes: low, medium, and high

## 2. Preprocessing
- Remove missing values
- Converted G3 into a categorial target
- G1-G3 were dropped
- Label encoded categorical variables
- Standardized features

##3. Part 2 - Algorithm Comparison

| Algorithm | Mean | Std |
| --------- | ---- | --- |
| Perception |  0.5674 | 0.0626 |
| Logistic Regression |  0.6341 | 0.0584 |
| KNN | 0.5910 | 0.0569 |
| Gaussian NB |  0.3720 | 0.0567 |
| Neural Network |  0.6105 | 0.0566 |

##4. Part 3 - Feature Selection

| Algorithm | Mean | Std |
| --------- | ---- | --- |
| Perception |  0.5938 | 0.0487 |
| Logistic Regression |  0.6698 | 0.0324 |
| KNN | 0.6369 | 0.0385 |
| Gaussian NB |  0.6354 | 0.0369 |
| Neural Network |  0.6477 | 0.0355 |

##5. Discussion

Feature selection improved all the models.
Logistic Regression had the best performance after selection.
Gaussian NB showed the most improvement due to reduced feature correlation.
KNN did well from reduced dimensionality.
Neural Network took the longest but improved from reduced noise.

The features selection was executed separately for each model instead of using the loop-based design
I first used. I did this because I wanted to manage the computational cost of each model. This led me to get
complete results from all the models in less time.

The desired output was not shown in the Python file due to my choice of testing each model separtely 
due to the really long runtime when trying to use all five. If the program is executed and the programmer 
has a lot of patience, the desired output should be displayed.

## 6. Reproduction
Python 3.12
Libraries: pandas, numpy, sklearn, ucimlrepo
Run the notebook from top to bottom
