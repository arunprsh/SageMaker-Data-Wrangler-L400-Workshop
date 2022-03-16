## Data Preparation

ML models are only as good as the data that is used to train them. In order to understand the nature/quality of data in hand, we need to start with exploratory data analysis (EDA). EDA helps you understand your data by identifying patterns in your data. For example, we might find that customers who book Resort hotels tend to stay longer than City hotels. Or customers that stay over the weekend purchase more meals. Because these patterns are not evident with data in tables, data scientists use visualization tools to help him identify patterns. 

Once you identify patterns in your data, you prepare your data enduring that suitable training data is available and is optimized for learning and generalization. You can prepare data using visual interactive tools like SageMaker Data Wrangler for data analysis and model building. Data Wrangler has no-code/low-code, automation, and visual capabilities to improve your data preparation productivity and to reduce the cost for interactive analysis.

Data preparation includes *data pre-processing* and *feature engineering*.

### Data Pre-processing

*Data preprocessing* puts data into the right shape and quality for training. Some data preprocessing strategies include: data cleaning, balancing, replacing, imputing, partitioning, scaling, augmenting and unbiasing etc.

* **Clean** (**replace, impute, remove outliers and duplicates)** — Remove outliers and duplicates, replace inaccurate or irrelevant data, and correct missing data using imputation techniques that will minimize bias as part of data cleaning.
* **Partition** — Randomly split data into train, validate, and test sets yo prevent ML models from overfitting and evaluate trained model accurately.
* **Scale (normalize, standardize)** — Having features on  normally distributed scale ensures that each feature is equally important. This will make it easier for many ML algorithms . Normalized numeric features have values between 0 and 1. Standardized numeric features better handle outliers and have a mean of 0 and standard deviation of 1.
* **Unbias, balance** **(detection & mitigation)** — Avoid inaccurate model results by detecting and mitigatin bias. An example of bias is if our dataset only includes hotel bookings from customer in a particular income range.
* **Augment** — Data augmentation increases the amount of data artificially by synthesizing new data from existing data. Data augmentation helps regularize data and reduces overfitting.

### Feature Engineering

After you explore and understand your data, you can move to *feature engineerin*g. Each data attribute is a feature such as the arrival date and time of checking in, length of stay, number of guests, and more. 

Feature engineering is a process to select and transform variables when creating a predictive model. Feature engineering typically includes feature creation, feature transformation, feature extraction, and feature selection.

**Feature creation** is creating new features from existing data to help with better predictions. Examples of feature creation techniques include: one-hot-encoding, binning, splitting, and calculated features.
**Feature transformation and imputation** manage replacing missing features or features that are not valid. Some techniques include: forming Cartesian products of features, non-linear transformations (such as binning numeric variables into categories), and creating domain-speciﬁc features.
**Feature extraction** involves reducing the amount of data to be processed using dimensionality reduction techniques like principle component analysis as an example (PCA). This reduces the required amount of memory and computing power , while still accurately maintaining original data characteristics.
**Feature selection** is the process of selecting subset of extracted features. This subset is relevant and contributes to minimizing the error rate of a trained model. Feature importance score and correlation matrix can be factors in selecting the most relevant features for model training.