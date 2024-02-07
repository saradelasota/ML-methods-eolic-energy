# ML-methods-eolic-energy
ML methods for forecasting eolic energy with sklearn. 

The dataset contains meteorological variables from 25 different locations near the eolic center in Sotavento.

Structure of the project:

0. Establishing inner and outer evaluation methods.
1. Assuring imputation improves performance.
   1.1 Compare a default imputation strategy (simple imputation with median strategy) to imputing the data set with 0 values.
2. Feature selection.
   2.1 We will employ simple imputation with median strategy and experiment with several data sets.
   2.2 Apply different methods select the best data set.
3. Gridsearch pipeline for each method.
   3.1 First setp involves the chosing of the imputation method, and the subsequent step involves the regressor.
   3.2 After establishing the range of search of the corresponding parameters, we will develop distinct pipelines for each method under 
       consideration (Decision tree, Knn regressor, Gradient Boosting and Random Forest).
   3.3 Select the best method based on the median absolute error and analize timing.
4. Hyperparameter optimization of the best two methods.
   4.1 We will create a pipeline for the three HPO methods (Random search, Halving search and Optuna) for the selected method.
   4.2 Analize the parameters obtained and the time of execution.
5. Selecting the final model.
   5.1 Estimate the accuracy of the final model using the outer evaluation.
   5.2 Train the final model and make predictions using the competition data set.
