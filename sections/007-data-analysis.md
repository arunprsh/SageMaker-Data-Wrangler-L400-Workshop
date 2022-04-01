## Analyze and Visualize 

Amazon SageMaker Data Wrangler includes built-in analyses that help you generate visualizations and data analyses in a few clicks. You can also create custom analyses using your own code.

You add an analysis to a dataframe by selecting a step in your data flow, and then choosing Add analysis. To access an analysis you've created, select the step that contains the analysis, and select the analysis.

All analyses are generated using 100,000 rows of your dataset.

You can add the following analysis to a dataframe:

    Data visualizations, including histograms and scatter plots.

    A quick summary of your dataset, including number of entries, minimum and maximum values (for numeric data), and most and least frequent categories (for categorical data).

    A quick model of the dataset, which can be used to generate an importance score for each feature.

    A target leakage report, which you can use to determine if one or more features are strongly correlated with your target feature.

    A custom visualization using your own code.




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

Let us create a prediction model on the fly using the raw crude features using Data Wrangler's Quick Model option.
A limit of 100,000 rows is used for this analysis. You can use the Quick Model feature to provide a rough estimate of the expected predicted quality and the predictive power of the features in your dataset. We don't recommend using a quick model to fine tune the data preprocessing pipeline or to optimize feature selection.

![quick-model-pre](.././img/quick-model-pre.png)