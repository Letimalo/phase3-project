Phase3-project: SyriaTel Customer Churn Project


<img src="telecommunications.jfif" alt="Telecommunications" width="600"/>
BUSINESS UNDERSTANDING

The problem statement for SyriaTel's customer churn dataset addresses a critical challenge faced by the telecommunications industry: predicting customer retention. As a binary classification problem, the goal is to determine whether a customer is likely to discontinue their business with SyriaTel in the near future. This prediction is crucial for mitigating financial losses associated with customer attrition. Telecommunication is a large sector which is steadily evolving providing various opportunities.

DATA UNDERSTANDING

The data contained in the dataset SyriaTel Customer Churn comprices of 3,332 rows and 21 columns as explained in the Jupyter notebook. It encompasses a range of customer metrics, including service usage, billing information, and customer plans, all crucial for predicting churn.

EXPLORATORY DATA ANALYSIS

Univariate analysis contains bar plot showing balance between churned and non-churned and histogram to see distribution of account lengths. For bivariate analysis; Boxplot to see how account length varies between churned and non-churned customers, boxplot to see how many minutes per day differs between curned and non_churned and boxplot to visualize how evening charges vary with churn. For multivariate; Pairplot of Features by Churn Status.

MODELLING

Different statistics tests such as chi-square and t-test were perfomed to analyse significance of the features to be used and also checking of correlation. There after transformation of categorical variables to numeric was done using one-hot encoding and label encoding in order to be able to create models. Next was dealing with data imbalance to ensure model is not going to overfit. First was splitting the data into train and test sets then performing resampling techniques which were SMOTE () and undersampling in that order. Then next was validating resampling impact by checking class distribution of resampled training data. Next was Re-evaluating feature importance to check if features used are relevant then scaling and cross-validation. Models that were made are Linear logistic regression as baseline model since it is a simple and effective linear model for binary classification tasks and random forest classifier model for multiple features because it is robust to overfitting and handles non-linear relationships well.

EVALUATING

Confusion matrix was used for both models and in logistic regression in the Confusion matrix, the instances model predicted correctly for both true negatives (572) and true positive (527) are much higher than when model predicted incorrectly false positive (27) and false negative (71). For random forest confusion matrix indicates that the instances model predicted correctly are significantly higher than the instances the model predicted incorrectly.

Logistic regression model has high precision, recall, and F1-scores for both classes with an accuracy of 92%. In random forest model performs excellently with high precision, recall, and F1-scores for both classes and also it has an accuracy of 95% indicating that it is highly effective in classifying both False and True instances. F1-scores are equal for both classes indicating a balanced performance between precision and recall for both classes.

CONCLUSION

The random forest model has an accuracy of 95% thus has strong predictive performance and both precision and recall are high.
From re-evaluating feature importance above, the top three features that are more important to model in the order of most important are 'total night charge', 'total day minutes' and 'customer service calls'.
