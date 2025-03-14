# Cap_Connectel
Customer Churn Prediction and Analysis

# Project Overview

This project aimed to analyze customer data, identify key factors influencing churn, and build a predictive model to help the business implement effective retention strategies. The insights derived from this project provide valuable guidance for improving customer satisfaction and loyalty.

### Data Collection and Loading

The dataset contained key customer details such as demographic information, service subscriptions, and billing data.

Data was imported into a Jupyter Notebook for cleaning, analysis, and model development.

### Data Cleaning and Preprocessing

Several steps were taken to ensure data quality and enhance model performance:

* Handling Missing Values

The TotalCharges column was originally imported as an object data type. This was corrected to numeric using 
/ pd.to_numeric() with errors='coerce'/

Missing values in the TotalCharges column were filled with the median to maintain consistency.

* Encoding Categorical Variables

Categorical features such as Gender, Contract, and PaymentMethod were encoded using Label Encoding and One-Hot Encoding for compatibility with machine learning models.

* Scaling Numerical Features

Features like Monthly Charges, Total Charges, and Tenure were scaled to ensure consistent feature ranges.

### Exploratory Data Analysis (EDA)

Key insights were drawn from visualizations and correlation analysis:

* Churn Analysis by Key Features

* Senior Citizens and customers with no partners showed higher churn rates.

* Customers using Electronic Check as a payment method exhibited the highest churn rate.

* Customers with Fiber Optic services and those without Tech Support experienced higher churn rates.

* Heatmap Analysis

Tenure showed a negative correlation with churn, reinforcing that long-term customers are less likely to leave.

Monthly Charges showed a positive correlation with churn, indicating that customers paying higher fees may be at higher risk.

### Model Building

Multiple machine learning models were evaluated to identify the best-performing model:

* Logistic Regression

* Random Forest Classifier

* XGboost

### Model Evaluation Metrics

* Accuracy provided a general measure of model performance.

* Recall was prioritized to minimize false negatives and ensure at-risk customers were accurately identified.

* Precision helped reduce false positives, ensuring retention resources were efficiently allocated.

* The F1-Score balanced precision and recall for optimal performance.

### Model Results and Insights

The confusion matrix heatmap revealed the following insights:

* The model effectively identified true positives (correctly predicted churners).The presence of false negatives indicated some churners were missed, Recall was prioritized to minimize missed churn cases and maximize retention efforts.

### Challenges Faced

Several challenges emerged during the project, which were addressed with appropriate strategies:

Data Type Errors: The TotalCharges column was imported as an object, requiring conversion to numeric for analysis.

Class Imbalance: The dataset had significantly fewer churn cases than non-churners. This was addressed using SMOTE to balance the classes.

### Key Recommendations

Based on the findings, the following actions are recommended:

* Implement proactive engagement strategies for new customers to reduce early churn.
* Offer tailored retention incentives for senior citizens and Electronic Check users, as they are identified as high-risk segments.
* Promote value-added services like Online Security, Tech Support, and Online Backup to improve retention.
* Improve customer onboarding and billing transparency to reduce dissatisfaction among high-paying customers with short tenure.

### Conclusion

This project successfully combined data cleaning, visualization, and machine learning techniques to predict customer churn. The insights derived offer actionable strategies for improving customer retention, reducing revenue loss, and enhancing overall business performance.
