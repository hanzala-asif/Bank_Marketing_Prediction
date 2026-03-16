# Bank Marketing - Term Deposit Subscription Prediction

## Task Objective
The primary objective of this task is to develop a predictive model that identifies whether a bank customer will subscribe to a term deposit as a result of a marketing campaign. This project addresses a binary classification problem by analyzing customer demographics, previous campaign interactions, and broader social-economic indicators. By accurately predicting subscription likelihood, financial institutions can optimize their marketing strategies, improve resource allocation, and enhance customer conversion rates.

## Approach and Methodology
The project follows a structured data science workflow, beginning with comprehensive **Data Exploration and Cleaning**. This phase involves analyzing the dataset's structure, verifying data integrity, and handling missing values or duplicates to ensure a robust foundation for modeling. Following data preparation, **Exploratory Data Analysis (EDA)** is conducted to uncover relationships between customer features—such as age, job type, and marital status—and the target subscription variable. Visualizations are employed to identify patterns and distributions that inform feature selection.

To prepare the data for machine learning, **Feature Engineering** is performed, which includes encoding categorical variables using `LabelEncoder` and scaling numerical features to improve model convergence and performance. The modeling phase involves training and comparing two distinct classification algorithms: **Logistic Regression**, which serves as a linear baseline, and **Random Forest**, a robust ensemble method capable of capturing complex, non-linear relationships within the data.

The models are rigorously evaluated using multiple performance metrics, including the **Confusion Matrix**, **F1-Score**, and **ROC Curve/AUC**, to ensure a balanced assessment of their predictive capabilities. Finally, the project incorporates **Model Interpretability (XAI)** using **SHAP (SHapley Additive exPlanations)**. This approach provides transparency into the model's decision-making process by identifying the most influential features for individual predictions and the overall model behavior.

## Results and Insights
The comparative analysis revealed that the **Random Forest** model generally outperformed Logistic Regression, demonstrating a superior ability to capture the nuances of customer behavior. Key insights derived from the analysis indicate that economic indicators, such as the **euribor3m** rate and the number of employees (**nr.employed**), are significant drivers of customer subscription. Furthermore, customers with specific professional backgrounds, such as administrative and technical roles, showed higher engagement with the campaign.

The use of SHAP values provided critical transparency, showing that the outcome of previous marketing campaigns and current economic stability are the primary factors influencing a customer's decision to subscribe. These findings suggest that banks should not only focus on individual customer demographics but also consider the broader economic context and historical interactions when designing marketing strategies.

## Repository Contents
| File Name | Description |
| :--- | :--- |
| `Bank_Marketing_Prediction.ipynb` | Complete Jupyter Notebook containing all code, visualizations, and detailed analysis. |
| `bank-direct-marketing-campaigns.csv` | The source dataset used for training and evaluating the predictive models. |
| `README.md` | A comprehensive summary of the project objectives, methodology, and key findings. |
