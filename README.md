# telecom_users_churn_analysis
Telecom churn analysis involves examining customer data to identify patterns and factors that lead to customer attrition, or churn, within a telecommunications company. A goal is to predict which customer is to leave the service and understand the reason behind their decisions.

# Requirements
Python 3.8+ Jupyter Notebook - Kaggle Notebook is preferrable.

# Dataset
Telecom churn Analysis: https://www.kaggle.com/datasets/alfathterry/telco-customer-churn-11-1-3/data

# How to Run The Notebook.
1. Login to Kaggle.com
2. Visit https://www.kaggle.com/datasets/alfathterry/telco-customer-churn-11-1-3/data link
3. Click on "New Notebook" Option Available on the top of the screen.
4. Download the ".ipynb" File attached in the current repository, select the right version
5. Upload On the New Notebook place by clicking on Import Notebook option.
6. Run The Notebook program

# Run the program in virtual envrionment python
1. Create virtual environment
2. Activate virtual environment
3. Install requirements.txt 
4. Run jupyter notebook and Open the .ipynb notebook file on the localhost:8888

# Key Data Insights
* In figure 1, we can see the count of customers who are leaving and those who are staying loyal to the service.
* In figure 2, it is observed that the length and width of the box is slightly (very tiny) is higher for **Price** and **Other**  value than that of **Competitors** , **Dissatisfaction** and **Attitude** value. And there is high variablity the churn category is equal to **Competitor**.

* In figure 3, it is observed that higher total charges are generally associated with higher churn rates as shown in **One Year** and **Two Year** Contract type. The influence of **Month-to-Month** contract shows that higher churn rate with lower median total chagres whereas long-term contracts like ony-year and two year tend to have churned customer with highere median total charges.Overall the plot suggest that customers on month-to-month contracts might need more motivation to stay, whereas customers on longer-term contracts who are paying higher charges might benefit from loyalty programs or discounts to reduce churn.
* In figure 4, it is observed that higher total charges are generally associated with higher churn rates as shown in **Fiber Optic** and **Cable** Internet type. The **Fiber Optic** Internet Type shows higher churn rate with lower median total charges as compared to **Cable** and **DSL**.
The customer's are prefering **Fiber Optic** Ineternet type than **Cable** and **DSL** irrespactive of churning.

* In figure 5, it is observed that there are more outlier's in when there is internet service.This indicates that there is higher variablity in total charges among the Customers.

* In figure 6, it is observed that the there is positive correlation between total charges and total revenue as it given that the total charges contribute to the total revenue.And the churned customers are relatively lower in number.

* In figure 7, it is observed that the majority of customer have stayed with service indicating high retention rate.But the count of newly joined customer is relatively to that of churned.

* CLTV means he value a customer contributes to your business over the entire lifetime at particular company. In figure 8 it shows that customer are staying for the services.

# Model Performance
4 Models has been trained and there result has been published below.
  1. LogisticRegression -  Accuracy Score - 96.34%
  2. RandomForestClassifier - Accuracy Score - 96.75%
  3. KNearestNeighbors - Accuracy Score - 74.94%
  4. XGBClassifier - Accuracy Score - 96.45%
     
Best Model as per below accuracy results can be considered as Random Forest and XGBoost as the second best model.

# Ethics Report
The RandomForestClassifier overfit the training data, making XGBoost the better choice. We need to fine-tune XGBoost's learning parameters to prevent overfitting.
