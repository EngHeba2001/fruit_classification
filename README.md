Fruit Classification using CatBoost
Project Overview

This project focuses on building a machine learning model to classify different fruit types using physical and descriptive attributes. The dataset contains approximately 10,000 records representing 20 fruit categories, including apples, bananas, oranges, mangoes, strawberries, watermelons, and others.

Dataset Features

The model uses the following input features:

Size (cm)
Weight (g)
Average Price (₹)
Shape
Color
Taste

Target Variable:

Fruit Name (20 classes)
Data Exploration and Preprocessing
Analyzed dataset structure and feature distributions.
Removed 246 duplicate records.
Verified that no missing values existed.
Identified outliers using the IQR method.
Applied logarithmic transformation to size and weight features to reduce skewness.
Split the dataset into training and testing sets using a 70/30 ratio.
Model Development

A CatBoost Classifier was implemented for multi-class classification due to its ability to efficiently handle categorical and numerical features without extensive preprocessing.

Model Parameters:

Iterations: 100
Learning Rate: 0.05
Depth: 6
Loss Function: MultiClass
Model Evaluation

The model achieved exceptional classification performance:

Accuracy: 100%
Precision: 100%
Recall: 100%
F1-Score: 100%

A 5-Fold Cross-Validation process was also conducted, demonstrating stable learning behavior and strong generalization performance across different folds.

Feature Importance

The most important features influencing fruit classification were:

Feature	Importance
Shape	31.57%
Average Price	23.35%
Weight	18.92%
Size	15.97%
Color	5.52%
Taste	4.66%

These results indicate that shape, price, and weight are the most influential factors in distinguishing fruit categories.

Technologies Used
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
CatBoost
Conclusion

This project demonstrates the effectiveness of CatBoost for multi-class fruit classification tasks. The model successfully classified 20 fruit categories with perfect accuracy, highlighting the strength of gradient boosting techniques in handling structured datasets containing both numerical and categorical features.
