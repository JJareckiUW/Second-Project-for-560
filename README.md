# Second-Project-for-560
Second Project for UW - Tacoma 560 Project. This was an end to end project using Breast Cancer data from mlbench

This contains two files: the RMD is the code for running multiple algorithms and classifiers using the breast cancer data set found in MLBench. All required packages are libraried as part of the initial code block.
The R code first imputes NAs using MICE, split into a training set and a hold out set, then begins multiple classifications/algorithms.
Algorithms and classifications used prior to ensemble techniques are support vector modeling, Naive Bayes, Neural Networks, decision tree, leave one out cross validation, regularised discriminant analysis, quadratic discriminant analysis, random forest, and boosting. Tables of accuracy, precision, and F1 scores are built for each model and compared.
Two ensemble techniques are used. First CaretEnsemble is used to combine decision tree, naive bayes, and neural net. Then, majority voting is used containing decision tree, naive bayes, neural net, random forest, and regularised discriminant analysis. The majority voting is compared to the other scores to determine which algorithms to try on the test set.
The test set is then run using neural net, regularised discriminant analysis, and amjority vote against the test set. The results are placed into a table with the train scores and compared to see which model is the best model to use against the data, as well as some analytic notes.
