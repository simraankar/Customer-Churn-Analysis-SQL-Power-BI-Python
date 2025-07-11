# Telco Customer Churn Analysis

#### by Simran Karmali

### Project Overview
This project explores and analyzes the Telco Customer Churn dataset from Kaggle to understand churn behavior and build a model to predict customer retention. It involves data cleaning, interactive dashboarding, and machine learning classification using the Random Forest algorithm.

### Tools & Technologies
<br> **SQL Server:** Data cleaning and preprocessing
<br> **Power BI:** Interactive dashboards and visualizations
<br> **Python (Jupyter Notebook):** Machine learning (Random Forest), feature analysis, and evaluation
<br> **Libraries:** pandas, matplotlib, seaborn, scikit-learn

### Dataset
The dataset [https://www.kaggle.com/datasets/blastchar/telco-customer-churn] contains detailed information about customers, their services, account details, and churn status. 
<br>
Telco Customer Churn dataset from Kaggle and cleaned it using SQL—this included handling missing values and converting the TotalCharges column from string to float. Also mapped the Churn column to binary values (Yes = 1, No = 0). The cleaned dataset was then imported into Power BI, where I created an interactive dashboard to visualize churn patterns, tenure, contract types, Internet service types, and Lifetime Value (LTV). After exploring insights in Power BI, I brought the cleaned data into Jupyter Notebook to build a Random Forest classification model. I split the data into an 80:20 train-test ratio and trained the model using 100 estimators with a random state of 42. Finally, I evaluated the model’s performance using precision, recall, F1-score, and accuracy metrics.
<br>
<br>
#### Model Evaluation - 
| Metric    | Class 0 (Retained) | Class 1 (Churned) |
| --------- | ------------------ | ----------------- |
| Precision | 83%                | 67%               |
| Recall    | 92%                | 46%               |
| F1-Score  | 87%                | 55%               |

Overall Accuracy: 80%
<br>
### Key Insights from Research Questions - 
<br> 1. Churned customers stay for an average of 18 months, while retained customers stay around 38 months — indicating longer-tenured customers are less likely to churn.
<br> 2. Fiber optic users show the highest churn rate (~42%), while DSL users churn moderately (~20%) and customers without internet service churn the least (~6%).
<br> 3. Month-to-month contract users churn the most (~45%), whereas one-year (~12%) and two-year (~2%) contract users are more loyal — proving long-term contracts reduce churn.
<br> 4. Retained customers have significantly higher LTV than churned ones, indicating that churned users generate less revenue over time.
<br> 5. Internet Service and Contract Type had the strongest influence on LTV, while Gender had negligible impact.
<br>
### Business Insights & Recommendations
Based on the analysis of churn behavior, tenure, contract types, and LTV, here are key insights and actions the business can take to reduce customer churn:

#### 1. Encourage Long-Term Contracts

* **Insight**: Customers on month-to-month plans have the highest churn (\~45%), while two-year contracts have the lowest (\~2%).
* **Recommendation**: Offer loyalty rewards, discounts, or perks to encourage longer contract commitments.

#### 2. Improve Experience for Fiber Optic Users

* **Insight**: Fiber optic users show the highest churn (\~42%) among all internet service types.
* **Recommendation**: Investigate pricing or service quality concerns and offer customized plans or customer support.

#### 3. Strengthen Early Customer Engagement

* **Insight**: Churned customers typically leave within the first 18 months.
* **Recommendation**: Focus on onboarding, regular engagement, and first-year incentives to retain new customers.

#### 4. Boost Lifetime Value Through Segmentation

* **Insight**: Contract type and Internet Service significantly affect LTV, while features like gender have little impact.
* **Recommendation**: Use segmentation and upselling strategies to improve LTV among low-value customers.

#### 5. Offer Proactive Technical Support

* **Insight**: Better service support is linked to higher tenure and retention.
* **Recommendation**: Introduce tech support plans and flag high-risk accounts for proactive outreach.

#### 6. Leverage Machine Learning for Early Churn Prediction

* **Insight**: The Random Forest model predicts churn with 80% accuracy.
* **Recommendation**: Use the model to trigger retention campaigns before customers decide to leave.



