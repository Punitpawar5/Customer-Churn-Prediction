# **Bank Customer Churn Prediction**

## **Introduction**
In today's competitive banking environment, customer retention is crucial for maintaining profitability and long-term growth. Predicting and mitigating customer churn, or attrition, can greatly benefit financial institutions by helping them sustain a loyal customer base and enhance revenue. This project aims to develop a machine learning model capable of predicting potential churners, thereby empowering banks to implement proactive retention strategies and optimize their resources.

## **Objective**
The primary objective of this project is to build a robust and accurate machine learning model to predict bank customer churn. By using historical data, the project aims to identify the main drivers of churn and generate actionable insights to minimize customer attrition.
<p align="center">
  <img src="https://github.com/Punitpawar5/Customer-Churn-Prediction/blob/main/customer-first.gif" alt="customer" width="200"/>
</p>

## **Project Phases**

### 1. Data Acquisition and Exploration
- **Data Overview**: The dataset includes **10,000 records** with **14 features**, covering customer details like **Credit Score, Geography, Gender, Age, Balance**, and more.
- **Exploratory Data Analysis (EDA)**: Initial univariate and bivariate analyses revealed that most customers are from **France** (5014), followed by **Germany** (2509) and **Spain** (2477). More **males** (5457) are in the dataset compared to females (4543).
- **Target Variable (Exited)**: The target variable represents customer churn status, where 1 indicates churn and 0 indicates retention. A class imbalance was observed, with more non-churners (5574) compared to churners (1426).

### 2. Data Preprocessing and Feature Engineering
- **Handling Missing Data**: The dataset was cleansed by dealing with missing values, inconsistencies, and outliers.
- **Encoding and Scaling**: Categorical features, like **Geography** and **Gender**, were encoded into numerical values to make them suitable for modeling. Feature scaling was also applied to standardize the numerical features.
- **Resampling**: To address the class imbalance, resampling techniques were used to create a balanced dataset with an equal number of churners and non-churners (1426 each).

### 3. Model Development
- **Algorithm Selection**: Several machine learning algorithms were explored, starting with the **Naive Bayes** model.
- **Cross-Validation and Hyperparameter Tuning**: Multiple models were trained with the aim of optimizing performance. Cross-validation techniques were used to ensure robust evaluation, while hyperparameter tuning refined the models.
- **Evaluation Metrics**: Models were evaluated based on metrics such as **accuracy, precision, recall, F1-score**, and **ROC-AUC**.

### 4. Model Interpretation and Insights Generation
- **Feature Importance**: After training the model, feature importance was analyzed to identify the key drivers of churn. Insights like customer **age, balance**, and **activity status** significantly influence whether a customer is likely to leave the bank.
- **Actionable Insights**: These insights can help stakeholders devise targeted retention strategies, such as personalized engagement efforts for customers with a high churn risk.
- **Validation**: Insights are validated using domain expertise to ensure practical relevance.

### 5. Model Deployment and Monitoring
- **Deployment**: Once the model is optimized and validated, it can be deployed into a production environment. Integration with **CRM systems** allows real-time predictions and proactive churn interventions.
- **Continuous Monitoring**: Continuous monitoring of key performance indicators (KPIs) like churn rates and customer satisfaction will ensure the model remains effective. Periodic recalibration will be required based on new data.

### 6. RESULT

#### Model Evaluation:

- Considering the intricacies of our dataset, we have assessed model performance primarily through the lens of recall and ROC-AUC metrics. 

- Recall is of particular importance due to its ability to minimize False Negative instances, while ROC-AUC provides insight into the model's overall class prediction accuracy.

- Among the models evaluated, AdaBoost emerges as the most favorable choice, showcasing exemplary recall and ROC-AUC scores of 0.998333 and 0.997827 on our test dataset, respectively.

#### Business Insights:

- Analysis reveals that female bank customers exhibit a higher churn rate at 11.4% compared to their male counterparts, who stand at 9%.

- Notably, customers aged between 40-50 demonstrate a heightened propensity to churn, registering a churn rate of 7.9%. This trend persists across other age demographics, with the 30-40 age group at 5.4%, 50-60 age group at 4.5%, those below 30 at 1.5%, and individuals above 60 at 1.1%.

- Geographically, both France and Germany record an identical churn rate of 8.1%, while Spain trails slightly behind at 4.1%.

- Active membership status significantly influences churn likelihood, with non-active members exhibiting a considerably higher churn rate of 13%.

- Further, customers possessing a credit card demonstrate a heightened churn propensity, with a churn rate of 14.2% compared to non-cardholders at 6.1%.

- Analysis also indicates that customers with Diamond card status exhibit a comparatively higher churn rate of 5.5%.

- Customers engaging in bank product purchases display a heightened churn rate of 14.1%, indicating potential areas for targeted retention strategies.

- Across satisfaction score brackets, we observe relatively balanced churn percentages ranging from 19-20%.

- Notably, all instances of churn are accompanied by customer grievances, underscoring the importance of addressing customer concerns to mitigate churn risk.

- Age, credit score, and balance distributions among churned and retained customers reveal nuanced similarities and differences, providing insights into customer behavior and preferences.


## **Conclusion**
The successful development of a predictive churn model enables banks to proactively identify at-risk customers and implement targeted retention strategies. This refined summary offers a comprehensive overview of model evaluation metrics and pertinent business insights, presented in a professional manner suitable for stakeholders and decision-makers. By leveraging machine learning techniques, financial institutions can improve customer satisfaction and drive long-term profitability and growth. These insights will help banks make data-driven decisions, enhance customer experience, and strengthen brand loyalty in a competitive marketplace.

---
