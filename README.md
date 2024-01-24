# Project Title :
Machine Learning-Predicting-Customer-Churn-Project.

## Project Overview :
This machine learning project focuses on predicting customer churn in the telecommunications industry. 
The goal is to build a model that can accurately classify whether a customer is likely to switch telecommunications providers, commonly referred to as "churning."

## Project Highlights :
  ### 1: Exploratory Data Analysis (EDA)

- Utilized various EDA techniques to understand the dataset.
- Applied univariate variable analysis using `df['feature'].unique()` to explore categorical features.

### 2: Feature Engineering

- Addressed issues in the dataset features, including fixing missing values and handling skewed distributions.
- Detected and transformed skewed distributions using log/sqrt transformations for numeric variables.

### 3: Encoding and Model Training

- Explored different encoding techniques, including CatBoost Encoding (Count Encoding, Target Encoding) and compared the performance with One-Hot Encoding.
- Scaled numeric data for improved model performance.
- Implemented a train/test split with a 70%/30% ratio and random_state=0 for reproducibility.
- Trained and evaluated machine learning models to achieve an accuracy on the test set of at least 0.90.

## Summary:

The project involved thorough exploratory data analysis, feature engineering, and model training to predict customer churn in the telecommunications industry. The following key points were observed:

- **Best Model:** Random Forest
- **Best Encoder:** Count Encoding
- **Best Metrics:** Precision, Recall, F1 Score
- **Best Scores:** See the table below for detailed metrics.

## Best Model Metrics:

| Best Model     | Best Encoder | Best Metrics | Best Score Macro | Best Score Micro | Best Score Weighted |
| -------------- | ------------ | ------------ | ---------------- | ---------------- | ------------------- |
| Random Forest  | Count        | Precision    | 0.969781         | 0.963137         | 0.963683            |
| Random Forest  | Target       | Precision    | 0.970513         | 0.959216         | 0.960286            |
| Random Forest  | CatBoost     | Precision    | 0.954677         | 0.95451          | 0.954525            |
| AdaBoost       | One Hot      | Precision    | 0.71221          | 0.863529         | 0.83091             |
| Random Forest  | Count        | Recall       | 0.875726         | 0.963137         | 0.963137            |
| ... (continued) | ...          | ...          | ...              | ...              | ...                 |

## Future Improvements:

While achieving an accuracy of 0.90 on the test set is a commendable goal, there are areas for improvement:

- Further feature engineering and selection could enhance model performance.
- Fine-tuning hyperparameters and exploring advanced ensemble methods might improve results.

## Best Encoding Performance:

The table above shows that Count Encoding with Random Forest achieved the highest precision, recall, and F1 scores on the dataset.

## Project Preview :
<img src="Images/best parametar.png">
