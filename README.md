🏆 Gold Recovery Optimization – Machine Learning Project

This project builds several machine learning models to predict the recovery rate of gold at different stages of the extraction process. The objective is to help a gold mining company improve production efficiency by identifying which model best predicts the final gold yield.

Using real industrial data from the recovery process, I built and evaluated Linear Regression, Decision Tree, and Random Forest models.
Model performance was evaluated using sMAPE (Symmetric Mean Absolute Percentage Error) — a more reliable metric for imbalanced values in rougher and final outputs.

🔍 Key Steps in the Project

Exploratory Data Analysis to understand process variables

Data preprocessing: handling missing values, feature selection, dataset structuring

Custom metric implementation (sMAPE) for rougher and final concentrate

Training and evaluating three different ML models

Hyperparameter tuning via GridSearchCV for Decision Tree and Random Forest

Comparing models using weighted sMAPE:

Rougher output weight: 0.25

Final output weight: 0.75

📊 Results & Model Comparison

Model performance (training sMAPE):

Linear Regression: ~8.96

Decision Tree: ~9.00

Random Forest: ~8.70 ← Best model

Random Forest performed the best overall due to its ability to capture nonlinear patterns and reduce error after tuning.
Decision Tree required careful parameter control to avoid overfitting.
Linear Regression provided stable results but lacked flexibility to capture complex relationships.

🎯 Final Recommendation

Based on sMAPE scores and generalization performance, Random Forest is recommended for operational use.
It provides the most accurate prediction of gold recovery, making it the most suitable model for production planning and optimization.

🧠 What I Learned

Handling real industrial data and domain-specific metrics

Implementing and interpreting custom evaluation metrics

Applying hyperparameter tuning effectively

Comparing models based on business impact, not just accuracy

Writing clear conclusions supported by metrics

