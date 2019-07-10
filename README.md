# Peer Lending Case Study - ML 95828 Spring 2019
In this study, we develop a series of machine learning models for evaluating peer lending investment opportunities. These models are trained and tested using historical data from loans that were issued on LendingClub between April 2008 and September 2017. It contains 750,000 loan listings with a total value exceeding $10.7 billion. The loan outcomes under consideration are predicted default rates and projected returns.

# Project Details
### Downloads
* Download the dataset from https://www.lendingclub.com/info/download-data.action
* Save the downloaded zip folder to your working directory and rename it "case_study_data.zip"

### Phase 1 - Research
Not shown in repository. Consisted of researching the subject, discussing goals, and brainstorming strategies.

### Phase 2 - Data cleaning
Prepares the LendingClub dataset for use in predictive models. The steps covered are:
1. Identify relevant features
2. Seperate features by datatype
3. Reading and combine data from several CSV's.
4. Remove invalid rows
5. Extract relavant features
6. Convert datatypes
7. Calculate yearly return for each loan using 3 different methods
8. Visualize data
9. Remove nulls and outliers
10. Visualize cross correlations
11. Ouput data "pickle", to be used in Phase 3

### Phase 3 - Model development and testing
Evaluates the predictive performance of several machine learning models on the Phase 2 dataset. In this notebook, we trained classifiers to predict loan defaults as well as regression models to predict returns on loans. The performance measures used in the classification section were accuracy (at best prediction % threshold), precision, recall, f1-score, ROC_AUC, and others. The best classification accuracy achieved was 80.3% (AUC = 0.7) using an L2 LogReg. The regression models were primary evaluated using R2 scores. The Random Forest Regressor performed the best out of these models with an r2 of 0.05. 

Classification Models:
* Naive Bayes
* L1 Logistic Regression
* L2 Logistic Regression
* Decision Tree
* Random Forest
* Multi-Layer Perceptron

Regression Models:
* L1 linear Regression
* L2 linear Regression
* Multi-layer Perceptron Regressor
* Random Forest Regressor


# Built With
* Anaconda 3.7
* Python Jupyter Notebooks
* Microsoft Office

# Authors
* Daniel Lesser
* Ghazal Erfani
* Joseph Standerfer

# Acknowledgments
* Professor Leman Akoglu (Carnegie Mellon University)
* Provost F, Fawcett T. (2013) Data Science for Business: What you need to know about data mining and data-analytic thinking. Sebastopol, CA: O'Reilly Media, Inc.
* Cohen MC, Guetta CD, Jiao K, Provost F. (2018) Data-driven investment strategies for peer-to-peer lending: a case study for teaching data science. Big Data 6:3, 191213, DOI: 10.1089/ big.2018.0092.
