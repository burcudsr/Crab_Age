# 🦀 Crab Age Prediction

This project focuses on regression analysis to predict the age of crabs based on physical measurements, utilizing data from the **Kaggle Playground Series: Season 3, Episode 16**. By applying targeted feature engineering and regression modeling, the project aims to achieve high predictive accuracy.

### 🚀 Live Demo
Explore the interactive prediction model here: **[Crab Age Prediction App](https://huggingface.co/spaces/bdaser/Crab)**

### 📊 Dataset & Preprocessing
The dataset consists of 74,051 training entries and 49,368 test entries, covering features such as sex, length, diameter, height, and various weight metrics. Key processing steps include:
* **Feature Engineering**: New domain-specific features were generated, including `Meat_Weight_Ratio` and a `Volume_Proxy` based on length, diameter, and height.
* **Data Cleaning**: Highly redundant features were removed to optimize the model structure.
* **Encoding**: One-hot encoding was applied to the 'Sex' column to maintain consistency across both training and test sets.

### 🤖 Model Performance
Various regression models were evaluated based on Mean Absolute Error (MAE), the official evaluation metric. The **Gradient Boosting** regressor was identified as the top-performing model.

| R-Squared | RMSE | MAE |
| :--- | :--- | :--- |
| 0.584 | 2.060 | 1.424 |
