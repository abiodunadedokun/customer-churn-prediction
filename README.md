# Customer churn prediction

---

#### Project Overview
This project aims to analyze and predict customer churn using machine learning techniques. By leveraging a telecommunication customer dataset, the goal is to identify patterns and factors contributing to churn and provide actionable insights to improve customer retention strategies.

---

#### Dataset Description
Data retrieved from Kaggle: [telco.csv](https://github.com/user-attachments/files/18290069/telco.csv)
<img width="950" alt="data" src="https://github.com/user-attachments/assets/18be5588-0c87-4d5d-a24e-3b09d2663c68" />

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
       <img width="950" alt="gender dist" src="https://github.com/user-attachments/assets/84485cf5-035c-4453-9cea-d6042ba777ea" />

     - Churn Rates by Gender
       <img width="950" alt="churn by gend" src="https://github.com/user-attachments/assets/1fa029bb-637b-4ea8-bfdf-ecee75c62883" />

     - Churn by Internet Service Type
       <img width="950" alt="churn by servi" src="https://github.com/user-attachments/assets/eaf2b521-1a6c-48e8-8b32-b310ae92d20a" />

     - Monthly Charges by Churn Status
     - <img width="950" alt="monthly" src="https://github.com/user-attachments/assets/4fe64457-9bd1-4806-bcbe-0171fc519127" />

     - Churn by Payment Method
     - <img width="950" alt="charge by pay" src="https://github.com/user-attachments/assets/715e1bf1-22ac-443a-b104-e217292ba128" />

     - Churn by Contract Type
     - <img width="950" alt="churn by con" src="https://github.com/user-attachments/assets/f4359211-57e1-46d0-84b5-f0da3c410130" />

     - Churn by Senior Citizen Status
       <img width="950" alt="churn by citi" src="https://github.com/user-attachments/assets/fa626d31-2de2-4821-8023-e7e99b226e25" />


2. Data Preprocessing:
   - Encoding categorical variables using Label Encoding.
   - Handling missing values by filling with the mean.
   - Ensuring all features are numeric for model compatibility.

3. Balancing the Dataset:
   - Addressing class imbalance using Synthetic Minority Oversampling Technique (SMOTE).

4. Feature Importance Analysis:
   <img width="950" alt="feat" src="https://github.com/user-attachments/assets/5a3f36b7-a0c2-4cf4-aefc-f617e4e4f504" />


6. Model Training and Evaluation:

   <img width="950" alt="res" src="https://github.com/user-attachments/assets/d5dc7152-735e-481e-b0f1-2031eeff1822" />

   - Model: Random Forest Classifier.
   - Performance Metrics:
     - Accuracy
     - Precision
     - Recall
     - F1-Score
   - Confusion Matrix Visualization.
   

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

