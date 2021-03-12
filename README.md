# Customer Churn Analysis

**Description:** The telecommunications company Telco is concerned about the number of customers leaving their landline business for cable competitors. They need to understand who is leaving and why. We analyze all relevant customer data to provide the marketing department with insights to develop focused customer retention programs.

About 26% of Telco’s customers left for cable competitors or due to other reasons. Customer retention costs cheaper for businesses rather than attracting new customers. A slight increase in the percentage of customer retention significantly increases sales and profits. Therefore, it is crucial to understand which customers are more likely to switch to competitors and identify the factors that influence the Telco customer churn rate by creating statistical models and conducting Exploratory Data Analysis. 

The identified factors are: Senior Citizen status, Internet Service type, Paperless Billing status, Payment Method, Tenure, Contract type, Monthly Charges and Dependents status. These factors need futher investigation with additional data. Based on this information, the company will be able to to develop a data-driven customer retention programs.

To predict Churn, We started of with a logistic regression model as a baseline model. We also use some minority oversampling in order to balance our dataset. Since only 27% of the records in our database were marked as “churned”, feeding our data into our algorithm without oversampling would have led it to underclassify our target variable. We used imblearn’s SMOTE to bring balance to our dataset.

Following the CRISP-DM methodology, we iterate by adding multiple features and compare with a Random Forest model. To identify the best model, we performed a randomized search and PCA to see if that had an influence and thereby pick the best performing model.

**Dataset source:** Kaggle

**Python Data Analysis libraries used:**
 - _NumPy_
 - _Pandas_
 - _sklearn_
 
**Python Data Visualization libraries used:**
 - _Matplotlib_
 - _Seaborn_
