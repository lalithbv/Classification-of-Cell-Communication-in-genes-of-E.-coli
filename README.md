# Binary Classification of Cell Communication in genes of E. coli bacterium

## Introduction

The primary aim of this project is to build a binary classifier using supervised machine learning algorithms that classifies if a gene of Escherichia coli or E.coli bacterium has the function “Cell communication” or not. E.coli is a common bacterium in the gut of humans and warm-blooded animals. Most E. coli strains have beneficial functions such as preventing the establishment of harmful bacteria in our intestine. However, there are pathogenic E. coli i.e., they can cause human illnesses like diarrhoea and even kidney failure. E. coli communicate by means of chemical signal molecules called autoinducers. This process, called “quorum sensing”, allows bacteria to count the members in the community and to change gene expression in the population synchronously. Successful bacterial–host interactions, both symbiotic and pathogenic, are frequently dependent on quorum-sensing-controlled processes.

## Data Specification

The data is given in CSV (Comma Separated Values) format with 1500 data points, one for each gene. The dataset has 116 features in total and one target column indicating whether the gene has the function “Cell communication” represented with binary labels 0 (Negative class) or 1 (Positive class). The first 103 columns describe the expression level of genes which are continuous (or numerical) values, and the following 13 columns are nominal (or categorical) features describing gene functional. 

**This dataset is uploaded as "Ecoli.csv".**

## Methodology
- Handled missing data using imputation based on target class and used Local Outlier Factor to remove outliers.
- Handled class imbalance by over-sampling using SMOTE and Standardized the data.
- Created voting classifier consisting of Logistic Regression, Random Forest, Support Vector Classifier, XG Boost and Gaussian Naive Bayes Classifier using K-fold CV.

## Result
- Got an average CV F1 score of  0.978 and an average CV accuracy of 0.978. 
- Received “Best Project Proposal" award.
