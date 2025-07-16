
Supervised ML
5 concepts: Data, Model, Training, Evaluation, Inference
Data = words, numbers in tables or pixels and waveforms. Dataset = cats, housing prices, weather info etc. Label = what all the features are measuring. Measure = what data you feed in to the ML model and its category. An ideal dataset has a large size and a lot of diversity to prevent the model from having biases. Evaluate a ML model by comparing its predictions to the actual values

train_test_split is a helper function from scikit. Its a random split that takes your data and splits it into training and testing set. you can set your test size/ training size. Cross validation is a way to solve the problem of needing a validation set. The simplest way = using cross_val_score which you can import from sklearn.model_selection.

then another function, cross_val_predict can be used to get predictions. the difference between the two mentioned functions is that the first one takes an average over CV folds and the second returns labels.
KFold is another function you can import that dvides all the samples in k groups of samples, these are all of equal sizes. RepeatedKFold repeats kfold n times w dif splits each time. As aforementioned, each split results in a dif testing/ training set. 
There are many types of splitting functions that are variations of kfold- some are more complex and some require each other in order to work.

Hyperparameters in scikit are things like c, kernell, gamma, and lasso for different models. 
