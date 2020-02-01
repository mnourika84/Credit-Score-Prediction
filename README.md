# Credit-Score-Prediction

•	Problem statement
o	Dataset: https://www.kaggle.com/c/GiveMeSomeCredit/data 
	cs-test.csv
	cs-training.csv

For this problem, the following steps completed to come up with an efficient prediction solution: 
At first, I did some preprocessing steps including dealing with imbalanced data, possible outliers,
missing values and standardization of the data of explanatory variables of train dataset and similarly 
over the test set. These steps presented in CreditScore-Preproccessing.ipynb file and output are saved 
in Traning_Set.xlsx and Test_Set.xlsx files .

Then, the train set split into two sets of train and validation with ratios of 80% and 20%. I compared 
the performance of several classification algorithms including Logistic Regression, SVM, Decision Tree, 
Random Forest, Gradient Boosting, K-Nearest Neighbor, Neural Network and Naïve Bayesian according to their 
default values of parameters and I found out Gradient Boosting (XGB) being the perfect candidate based on 
the accuracy measurements of these methods over train and validation datasets using 2-fold cross validation.

Then the hyperparameters of XGB were tuned using Grid Search with the accuracies of 83% over train and 84% 
over validation. These steps are available in CreditScore_Classification.ipynb file.


Finally, the probability of default over the test set observations saved in Prediction_results.xlsx
file.

The end! 
