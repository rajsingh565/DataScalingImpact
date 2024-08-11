## Introduction
This project is designed to analyze and understand how scaling affects the performance of machine learning models. Worked with the Social_Network_Ads.csv dataset, where the goal is to predict if a user purchased a product based on their age and salary.

## Dataset
The dataset consists of 400 records with three columns:

Age: The age of the user.
EstimatedSalary: The estimated salary of the user.
Purchased: A binary indicator of whether the user purchased the product (1 for yes, 0 for no).
Data Preprocessing
We performed the following steps in data preprocessing:

Feature Selection: Selected the relevant features (Age and EstimatedSalary) and the target variable (Purchased).
Train-Test Split: The dataset was split into training and testing sets with a 70-30 ratio using train_test_split.
Feature Scaling
Feature scaling was applied using StandardScaler to standardize the features. This transformation was crucial for ensuring that the machine learning models trained effectively, especially for models like logistic regression which are sensitive to the scale of input data.

 ## Effect of Scaling
Visualizations were generated to show the effect of scaling:

Scatter plots comparing the data before and after scaling.
KDE plots to compare the distribution of features before and after scaling.
Exploratory Data Analysis
Before and after scaling, we analyzed the data distribution:

Age Distribution: Visualized the age distribution before and after scaling.
Estimated Salary Distribution: Visualized the salary distribution before and after scaling.
These visualizations highlighted the importance of scaling in ensuring that the data is standardized for effective model training.

## Machine Learning Models
Two models were trained and evaluated:

Logistic Regression: A linear model used for binary classification.
Decision Tree Classifier: A non-linear model that splits the data into decision nodes based on the features.
Model Training and Evaluation
Both models were trained using the original (unscaled) data and the scaled data:

Logistic Regression: Improved performance with scaled data.
Decision Tree Classifier: Performance remained consistent regardless of scaling, demonstrating the tree model's inherent robustness to feature scaling.
Effect of Outliers
To analyze the impact of outliers:

Introduced outliers in the dataset by adding extreme values for Age and EstimatedSalary.
Visualized the data before and after scaling to observe the effect of outliers.
Retrained the models to see if the performance was affected by the presence of outliers.
## Results
## Logistic Regression Accuracy:
Unscaled data: 65.83%
Scaled data: 86.67%
## Decision Tree Classifier Accuracy:
Unscaled data: 87.50%
Scaled data: 87.50% , 

These results emphasize the importance of scaling for models like logistic regression, while decision trees are generally unaffected by scaling.

## Conclusion
This project demonstrated the significance of data preprocessing and scaling in training effective machine learning models. The logistic regression model showed substantial improvement when scaling was applied, while the decision tree model remained unaffected. Additionally, the impact of outliers was explored, providing insights into how they can distort the analysis if not appropriately handled.
