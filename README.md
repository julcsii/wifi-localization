# minodes
Data science challenge for MiNODES internship position.

ML task: Supervised learning>Multilabel classification problem.

Observations: High dimensionality problem, Lot of 0 values, too many labels to predict, curse of dimensionality (not enough data)

Validation set vs trainig set: Since the test data does not contain any targets, I divide the traning set into validation set and training set. (50% training, 25% validation, 25% test)

Pre-processing: 
- Feature extraction: sklearn.feature_extraction.DictVectorizer>fit_transform() 
- Feature selection: 
	- Features: received signal strength indication (RSSI) of wifi nodes (137) from which we select ???? most relevant features with sklearn.feature_selection.SelectKBest
	- Labels: Compartments of store (96)
 
Dimensionality reduction: Principal component analysis - not useful, the components are barely correlating with the selected relevant features (correlation is negative)

Potential prediction techniques: Nearest neighbour calssification, Decision trees, SVM, Naive bayes, Neural networks
I chose ???????

Model selection:
- Model validation metrics: Mean Absolute Error, Bias, Variance, confusion matrix, accuracy, precision, f1 score, recall, information gain, entropy
http://scikit-learn.org/stable/modules/model_evaluation.html#classification-metrics

- Grid search


Future enhancements: k-folds Cross-validation, regularization, hyper parameter fine-tuning

Conclusion:

Implemented with Python 3.6.2 :: Anaconda custom (64-bit)

Used libraries: ast, pandas, numpy, sklearn



