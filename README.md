# Domain classifier task

The notebook `1_EDA_FeatureSelection.ipynb` contain data cleaning code and a simple exploratory data analysis.
In notebook `2_Classification.ipynb` the data has been classified using suggested columns by mutual information ranking, however the algorithm is overfitting.
3rd notebook contains another approach based on previously carried out experiments, that is selection of numerical features along with dropping of nulls/nans. 
By doing so, and disregarding balancing the dataset with SMOTE/SMOTETokem, XGBoost (w/o hyperparameter tuning) achieved 76% F1 Score, 76% Balanced Accuracy, 87% ROC AUC on a validation set (the set is not highly representative, it contains 200 samples from each group).
