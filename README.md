# Insurance Claim Fraud Detection using Machine Learning

This project develops a machine learning system to detect fraudulent insurance claims. It applies data preprocessing, exploratory data analysis, and multiple ML algorithms to build a predictive model that can classify claims as legitimate or fraudulent.The final outcome is a fraud detection model that can support insurance companies in minimizing financial losses and improving risk management.


# About the DataSet

This dataset is from a project at Indian Institute of Management Calcutta, contains 1,000 insurance claim records labeled as fraudulent or legitimate.
It includes customer demographics, policy information, incident details, vehicle data, and claim amounts, with 38 explanatory features and 1 target variable (fraud_reported). This makes it well-suited for developing and evaluating machine learning models for insurance fraud detection.


## 🔄 Project Workflow

1. **Data Understanding & EDA**
   - Explored the dataset to understand distributions, fraud patterns, and correlations.
   - Visualized fraud vs. legitimate claims and key influencing factors.

2. **Data Preprocessing**
   - Cleaned missing values and inconsistent entries.
   - Encoded categorical variables.
   - Scaled numerical features where required.
   - Applied **SMOTE** to handle imbalanced classes.

3. **Feature Engineering**
   - Extracted important features such as claim ratios and accident severity.
   - Prepared input features for machine learning models.

4. **Model Training**
   - Trained multiple ML models:
     - Logistic Regression  
     - Decision Tree  
     - Random Forest  
     - Gradient Boosting  

5. **Model Evaluation**
   - Compared models using:
     - Accuracy  
     - Precision  
     - Recall  
     - F1-Score  
     - ROC-AUC  
   - Visualized performance with confusion matrix and ROC curves.

6. **Model Selection & Interpretation**
   - Selected **Random Forest** for balanced precision and recall.  
   - Used **SHAP** to interpret predictions and identify key fraud indicators.
  

## 📈 Results

Several machine learning models were trained and evaluated on the insurance fraud dataset.  
The performance was measured using Accuracy, Precision, Recall, F1-Score, and ROC-AUC.  

| Model               | Accuracy | Precision | Recall | F1-score | ROC-AUC |
|----------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.545    | 0.306     | 0.673  | 0.420    | 0.608   |
| Decision Tree       | 0.830    | 0.623     | 0.776  | 0.691    | 0.819   |
| Random Forest       | 0.820    | 0.633     | 0.633  | 0.633    | 0.816   |
| Gradient Boosting   | 0.815    | 0.625     | 0.612  | 0.619    | 0.806   |

### 🔎 Key Insights
- **Logistic Regression** performed poorly, highlighting the complexity of fraud detection.  
- **Decision Tree** achieved the highest recall, making it strong at identifying fraudulent cases.  
- **Random Forest** provided a balanced trade-off between precision and recall with a strong ROC-AUC.  
- **Gradient Boosting** delivered comparable performance to Random Forest.  

✅ **Final Model Chosen**: **Random Forest**  
- Accuracy: ~82%  
- Balanced precision & recall  
- ROC-AUC: ~0.82  
- Interpretable with SHAP feature importance  


## ✅ Conclusion

This project demonstrates how machine learning can be applied to detect fraudulent insurance claims, a critical challenge in the financial and insurance industry.  

- Exploratory Data Analysis (EDA) revealed key fraud patterns related to claim amounts, incident severity, and policy details.  
- Multiple models were trained, and **Random Forest** was selected as the final model for its balanced performance across precision, recall, and ROC-AUC.  
- The model achieved **~82% accuracy** and a **ROC-AUC score of 0.82**, making it reliable for real-world fraud detection.  
- With the use of SHAP, the project also provided **model interpretability**, highlighting important fraud indicators such as claim amounts and policy premiums.  

Overall, this project shows that machine learning can effectively support **insurance companies** in minimizing losses from fraudulent claims while ensuring genuine claims are processed smoothly.  


