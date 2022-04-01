## Analyze and Visualize 

Amazon SageMaker Data Wrangler includes built-in analyses that help you generate visualizations and data analyses in a few clicks. You can also create custom analyses using your own code.

You add an analysis to a dataframe by selecting a step in your data flow, and then choosing Add analysis. To access an analysis you've created, select the step that contains the analysis, and select the analysis.

All analyses are generated using 100,000 rows of your dataset.

You can add the following analysis to a dataframe:

* Data visualizations, including histograms and scatter plots.
* A quick summary of your dataset, including number of entries, minimum and maximum values (for numeric data), and most and least frequent categories (for categorical data).
* A quick model of the dataset, which can be used to generate an importance score for each feature.
* A target leakage report, which you can use to determine if one or more features are strongly correlated with your target feature. 
* A custom visualization using your own code.


### Target Leakage 
![target-leakage](.././img/target-leakage.png)

### Feature Correlation (Linear)
![linear-pre](.././img/linear-pre.png)


### Feature Correlation (Non-Linear)
![non-linear-pre](.././img/non-linear-pre.png)


### Multicolinearity Inflation Variance Factors
![variance-inflation-factors-pre](.././img/variance-inflation-factors-pre.png)


### Multicolinearity Principal Component Analysis (PCA)
![pca-pre](.././img/pca-pre.png)


### Multicolinearity Lasso Feature Selection 
![lasso-pre](.././img/lasso-pre.png)


### Detect Duplicate Rows
![duplicate](.././img/duplicate-2.png)


### Quick Model

Use the Quick Model visualization to quickly evaluate your data and produce importance scores for each feature. A feature importance score indicates how useful a feature is at predicting a target label. The feature importance score is between [0, 1] and a higher number indicates that the feature is more important to the whole dataset. On the top of the quick model chart, there is a model score. A classification problem shows an F1 score. A regression problem has a mean squared error (MSE) score.

When you create a quick model chart, you select a dataset you want evaluated, and a target label against which you want feature importance to be compared. Data Wrangler does the following:
* Infers the data types for the target label and each feature in the dataset selected.
* Determines the problem type. Based on the number of distinct values in the label column, Data Wrangler determines if this is a regression or classification problem type. Data Wrangler sets a categorical threshold to 100. If there are more than 100 distinct values in the label column, Data Wrangler classifies it as a regression problem; otherwise, it is classified as a classification problem.
* Pre-processes features and label data for training. The algorithm used requires encoding features to vector type and encoding labels to double type.
* Trains a random forest algorithm with 70% of data. Spark’s RandomForestRegressor is used to train a model for regression problems. The RandomForestClassifier is used to train a model for classification problems.
* Evaluates a random forest model with the remaining 30% of data. Data Wrangler evaluates classification models using an F1 score and evaluates regression models using an MSE (mean squared error) score.
* Calculates feature importance for each feature using the Gini importance method.

Let us create a prediction model on the fly using the raw crude features using Data Wrangler's Quick Model option.

A limit of 100,000 rows is used for this analysis. You can use the Quick Model feature to provide a rough estimate of the expected predicted quality and the predictive power of the features in your dataset. 

![quick-model-pre](.././img/quick-model-pre.png)