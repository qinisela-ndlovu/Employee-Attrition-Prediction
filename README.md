### HR Employee-Attrition-Prediction 
In this project I aimed to predict employee attrition: a challenging and imbalanced classification problem. 

### Project Goals
- Understand patterns of employee attrition.
- Build and evaluate the model to predict attrition.
- Explain predictions.

### Tools & Technologies
- Python: Pandas, NumPy, Scikit-learn, XGBoost,Random Forest ..)
- Data visualisation: Matplotlib, Seaborn
- Jupyter Notebook

### Dataset Source
- IBM HR Data Analytics from Kaggle


-This is the same dataset I used in  a previous exploratory  data analysis project(HR).
-but here the focus is on building a predictive model, evaluate its performance.

### Project Structure
- Employee Atrrition Prediction : Jupter notebook  for data cleaning, modelling and interpretation
- data -: dataset file(s)
- README.md : Employee Attrition Project Overview

### Results 
Data Prep  & Pipeline Design:
- I converted the target var to binary and carefully selected features, removing the ones causing multicollinearity
- I build the pipeline integrating preprocessing, SMOTE oversampling to handle the imbalance and classifier - ensuring cleaner code and reproducible model training.

XGBoost Modelling:
- I started with a baseline XGBoost using default parameters, results were not good so I implemented a GridSearchCV pipeline to tune the parameters.
- Delivered a good balance between accuaracy and recall for minority(1) class, using SMOTE
- Threshold tuning improved the recall, enhancing iits ability to detect who might leave

Random Forest Modelling:
- I used it  as a benchmark, with a similar training and tuning process.
- Performed slightly worse than XGBoost but still provided useful insights to me.
- Threshold adjustment also increased the recall, confirming its impact across models.

Evaluation and Insights:
- The graphs(Precision-recall curves and average precision scores) (XGBoost ~0.55, RF ~0.48) showed moderate predictive power.
- Highlighted the recall-precision tradeoff and the role of threshold tuning in handling imbalanced data.
- Both models are viable for real-world use, though further feature engineering and imbalance handling could be useful for better results

### Future work
- This was iterative work, not just modelling.
- I plan to explore additional models like LightGBM(still learning), incorporate domain knowledge for feature engineering and expirement with cost-sensitive learning to better captre the business impact of attrition predictions.
- 
### License
This project is for educational(work) and research purposes only. The data I used belongs to IBM/kaggle.


