# Customer churn prediction

---

#### Project Overview
This project aims to analyze and predict customer churn using machine learning techniques. By leveraging a telecommunication customer dataset, the goal is to identify patterns and factors contributing to churn and provide actionable insights to improve customer retention strategies.

---

#### Dataset Description
Data retrieved from Kaggle: [telco.csv](https://github.com/user-attachments/files/18290069/telco.csv)

The dataset contains customer information from a telecommunications company. It includes:

1. Demographic Data:
   - Gender: Male or Female.
   - Senior Citizen: Whether the customer is a senior citizen (1) or not (0).

2. Account Information:
   - Tenure: Number of months the customer has stayed with the company.
   - Contract Type: Type of contract (e.g., Month-to-month, One year, Two year).
   - Payment Method: Method used by the customer for payments (e.g., Electronic check, Mailed check, Bank transfer (automatic), Credit card (automatic)).

3. Service Information**:
   - Internet Service: Type of internet service (e.g., DSL, Fiber optic, None).
   - Phone Service: Whether the customer has a phone service (Yes/No).
   - Streaming Services: Whether the customer has streaming TV or streaming movies (Yes/No).

4. Billing Information:
   - Monthly Charges: The amount charged to the customer monthly.
   - Total Charges: The total amount charged to the customer over the tenure period.

5. Target Variable:
   - Churn: Indicates whether the customer churned (Yes/No).

The dataset contains 7,043 records, providing a comprehensive view of customer behaviors and preferences.

---

#### Project Structure
The project is divided into the following key sections:

1. Exploratory Data Analysis:
   - Visualizations provide insights into customer distribution and churn patterns.
   - Key charts:
     - Gender Distribution
     - Churn Rates by Gender
     - Churn by Internet Service Type
     - Monthly Charges by Churn Status
     - Churn by Payment Method
     - Churn by Contract Type
     - Churn by Senior Citizen Status

2. Data Preprocessing:
   - Encoding categorical variables using Label Encoding.
   - Handling missing values by filling with the mean.
   - Ensuring all features are numeric for model compatibility.

3. Balancing the Dataset:
   - Addressing class imbalance using Synthetic Minority Oversampling Technique (SMOTE).

4. Model Training and Evaluation:
   - Model: Random Forest Classifier.
   - Performance Metrics:
     - Accuracy
     - Precision
     - Recall
     - F1-Score
   - Confusion Matrix Visualization.
   - Feature Importance Analysis.

---

#### Results
- Model Accuracy: ~85%
- Key Insights:
  - Higher churn rates for customers with higher monthly charges.
  - Significant churn differences based on contract type and internet service.
  - Electronic check payment method correlates with higher churn.

---

### Recommendations Based on Business Insights

1. **Insight:** Senior customers are more likely to churn.  
   - Recommendation: Develop senior-specific retention strategies, such as offering simplified plans, personalized communication, or exclusive discounts tailored to their needs.

2. **Insight:** Customers with higher monthly charges exhibit increased churn rates.  
   - Recommendation: Introduce loyalty programs, bundle discounts, or promotional offers to reduce the perceived burden of monthly charges and enhance value perception.

3. **Insight:** Customers using "Electronic Check" as a payment method have the highest churn rates.  
   - Recommendation: Provide incentives to switch to automated payment methods like "Credit Card (Automatic)" or "Bank Transfer" to ensure payment consistency and reduce churn.

4. **Insight:** Short-term or month-to-month contract customers are more prone to churn.  
   - Recommendation: Encourage longer-term contracts by offering incentives such as reduced rates, additional benefits, or exclusive perks for annual plans.

5. **Insight:** Customers using "Fiber Optic" internet service are more likely to churn.  
   - Recommendation: Improve service reliability and performance for fibre optic users. Launch customer satisfaction surveys to identify pain points and implement enhancements.

