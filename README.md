# Titanic Machine Learning Model: Random Forest & Logistic Regression

## Project Summary

This project explores machine learning techniques for predicting the survival of passengers aboard the Titanic. The primary focus is on applying **Random Forest** and **Logistic Regression** models to the Titanic dataset using the **tidymodels** package in R. The Titanic dataset is a well-known dataset that contains information about passengers, including whether they survived or not, and various attributes such as age, class, sex, and the number of siblings/spouses aboard.

The project aims to compare the ***performance of both models*** and evaluate their **effectiveness** in predicting passenger `survival`.

## Objective

The objective of this project is to:
- Build two predictive models (Random Forest and Logistic Regression) to predict passenger survival on the Titanic.
- Use the **tidymodels** package in R to create, train, and evaluate the models.
- Compare the performance of both models using appropriate evaluation metrics.
- Analyze the results and draw conclusions about the models' effectiveness in predicting Titanic survival.

## Study Plan & Steps

### Step 1: Data Exploration and Preprocessing
- **Load the Titanic dataset** from the `titanic` package or directly from a CSV file.
- **Examine the dataset** to understand its structure, missing values, and outliers.
- Perform **data cleaning**: Handle missing values, outliers, and any necessary transformations on categorical variables (e.g., encoding 'Sex', 'Embarked').
- **Feature Engineering**: Create new features, such as family size age, and possibly remove redundant or irrelevant features.

### Step 2: Data Splitting
- Split the dataset into training and testing sets using a 80/20 split.
- Create resampling strategies for model validation, such as **cross-validation** using the `vfold_cv` function.

### Step 3: Model Building & Training
- **Random Forest Model**:
  - Use `rand_forest()` from **tidymodels** to define and train the Random Forest model.
  - Tune the hyperparameters using grid search or random search.
  
- **Logistic Regression Model**:
  - Use `logistic_reg()` from **tidymodels** to define and train the Logistic Regression model.

### Step 4: Model Evaluation
- Evaluate the models using appropriate metrics such as accuracy, and AUC.
- Compare the performance of the two models using the testing set and resampling methods.
- Visualize the confusion matrix and ROC curves for both models.

### Step 5: Interpretation and Conclusion
- Analyze the importance of the variables in both models, especially for the Random Forest model.
- Discuss which features contribute most to the survival prediction.
- Evaluate the results in terms of model performance and interpretability.

## Conclusion & Next Steps

### Conclusion:
- Both models demonstrated the ability to predict Titanic survival, with **Random Forest** potentially providing higher accuracy due to its flexibility with non-linear relationships between features.
- Logistic Regression is simpler and more interpretable, which is useful for understanding how individual variables contribute to predictions.

### Next Steps:
- Further **hyperparameter tuning** could be explored for `Logistic Regression` models to optimize their performance.
- Investigate other machine learning algorithms (e.g., Support Vector Machines, K-Nearest Neighbors) to compare with the current models.
- Apply advanced feature engineering techniques to enhance model performance, such as interactions between features.
- Implement model performance monitoring to track real-time performance if the model is deployed in production.

## Technologies Used
- **R** programming language
- **tidymodels** package for machine learning
- **randomForest** for Random Forest modeling
- **ggplot2** for data visualization

## Dependencies
- `tidymodels`
- `titanic`
- `ggplot2`
- `randomForest`
- `dplyr`
