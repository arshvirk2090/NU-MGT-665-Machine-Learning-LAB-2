# Predictive Model Evaluation Report

## Introduction
This repository contains a comprehensive analysis of a predictive model's performance in forecasting student withdrawals within an educational context. The model considers various predictor variables such as module codes, demographic factors, educational backgrounds, and socioeconomic indicators. The evaluation includes key metrics, interpretation of coefficients, confusion matrix analysis, resampling outcomes, and suggestions for model improvements.

## Interpretation of Coefficients
The coefficients of predictor variables are analyzed to understand their impact on withdrawal likelihood. Modules BBB, CCC, DDD, and FFF, along with presentations in 2014B, exhibit significant positive effects on withdrawal, while male gender (genderM) has a significant negative effect. Certain regions and educational backgrounds also influence withdrawal likelihood, with higher deprivation bands associated with increased withdrawal rates.

## Performance Metrics
The predictive model achieved an accuracy of approximately 70.28%. Precision, recall, and F1 score provide nuanced insights, with precision at around 52.77%, recall at approximately 17.00%, and F1 score at 25.71%, indicating moderate overall performance.

## Confusion Matrix
The confusion matrix offers a detailed breakdown of the model's predictions:

|                      | Predicted Negative (0) | Predicted Positive (1)|
|----------------------|------------------------|-----------------------|
| Actual Negative (0)  | 2051                   | 145                   |
| Actual Positive (1)  | 791                    | 162                   |

## Area Under the Curve (AUC) Metrics
- The AUC-ROC (Area Under the Receiver Operating Characteristic Curve) value of approximately 0.666 suggests that the model has a moderate ability to distinguish between the positive and negative classes. A higher AUC-ROC indicates better discrimination, so a value of 0.666 indicates that the model performs better than random chance (where AUC-ROC = 0.5), but there is room for improvement.

- The AUC-PR (Area Under the Precision-Recall Curve) value of around 0.571 suggests a moderate balance between precision and recall. This means that the model strikes a fair equilibrium between accurately identifying positive instances and capturing all positive cases within the dataset.

## Resampling Results
Resampling outcomes show an average RMSE of approximately 0.4457 units and an R-squared value of approximately 0.0818, indicating the model explains only about 8.18% of the variance. The MAE is approximately 0.3969, suggesting relatively close alignment between predictions and actual values.

## Conclusion
The predictive model for student withdrawals in education demonstrates moderate performance, with strengths in distinguishing classes and balancing precision and recall. However, it exhibits weaknesses in explaining variance, indicating potential areas for improvement.

Please run the code "MGT 665 LAB-2.R" for analysing the outcome given in the report. 
