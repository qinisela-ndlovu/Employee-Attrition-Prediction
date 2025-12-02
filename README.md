### HR Employee-Attrition-Prediction 
This project predicts employee attrition (whether an employee will stay or leave) using machine learning models. The goal is to demonstrate an end-to-end workflow including data preprocessing, modeling, and evaluation.

### Project Goals
- Understand patterns of employee attrition.
- Build and evaluate the model to predict attrition.
- Explain predictions.

### Tools & Technologies
- Python: Pandas, NumPy, Scikit-learn, XGBoost,Random Forest )
- Data visualisation: Matplotlib, Seaborn
- Jupyter Notebook

### About Data
- Synthetic Data
- Features: 30+ employee-related variables (numeric and categorical)
- Target variable: Attrition (Yes/No)
  
## Workflow
 1. Data Preprocessing
    - Selected relevant features
    - Handled numeric and categorical variables separately
    - Split data into training (80%) and testing (20%) sets
    - Applied SMOTE to balance classes for better prediction of minority class
  2. Modelling
     - Random Forest
     - XGBoost Classifier
     - Used Pipelines to combine preprocessing and modelling
  3. Evaluation
     - Metrics used: Accuracy, Precision, Recall, F1-score
     - Confusion matrices for visualizing predictions
     - Observed trade-offs in predicting the minority class (employees likely to leave)
   

### Project Structure
- Employee Atrrition Prediction : Jupyter notebook  for data cleaning, modelling and interpretation
- data : dataset file(s)
- README.md : Employee Attrition Project Overview

### Key Results
| Model         | Accuracy | Precision (Yes) | Recall (Yes) | F1-score (Yes) |
| ------------- | -------- | --------------- | ------------ | -------------- |
| Random Forest | 0.84     | 0.53            | 0.49         | 0.51           |
| XGBoost       | 0.84     | 0.55            | 0.47         | 0.51           |

Please Note: "YES" refers to employee predicted to leave. SMOTE was appplied to address class imbalance.

# Conclusion:
This project demonstrates:
- Handling of numeric and categorical features
- Use of pipelines and SMOTE for imbalanced data
- Training and evaluation of multiple models
- Interpretation of model performance using standard metrics

### Future work
- Hyperparameter Tuning: Optimize Random Forest and XGBoost using grid search or randomized search to improve model performance.
- Feature Engineering: Create new features or aggregate existing ones to capture employee behavior patterns more effectively.
- Cross-Validation: Implement k-fold cross-validation to get more robust performance estimates



