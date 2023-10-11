# Domain classifier task

The notebook `1_EDA_FeatureSelection.ipynb` contain data cleaning code and a simple exploratory data analysis.

In notebook `2_Classification.ipynb` the data has been classified using suggested columns by mutual information ranking, however overfitting of the algorithm is observable.

3rd notebook `3_FeaturesSelectionDropApproach.ipynb` contains different approach based on previously carried out experiments, that is selection of numerical features along with dropping of nulls/nans.

By doing so, and disregarding balancing the train dataset with SMOTE/SMOTETomek, XGBoost (w/o hyperparameter tuning) achieved 76% F1 Score, 76% Balanced Accuracy, 87% ROC AUC on a validation set (the set is not highly representative, it contains 200 samples from each group). The results are available in `4_XGB_DropScaleWeights.ipynb`.

After hyperparameters tuning, the algorithm performace increased to 80% F1 Score, 80% Balanced Accuracy, and 90% ROC AUC.
