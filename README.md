# Predictive Model Evaluation Report

## Introduction
This repository contains a comprehensive analysis of a predictive model's performance in forecasting student withdrawals within an educational context. The model considers various predictor variables such as module codes, demographic factors, educational backgrounds, and socioeconomic indicators. The evaluation includes key metrics, interpretation of coefficients, confusion matrix analysis, resampling outcomes, and suggestions for model improvements.

## Interpretation of Coefficients
The coefficients of predictor variables are analyzed to understand their impact on withdrawal likelihood. Modules BBB, CCC, DDD, and FFF, along with presentations in 2014B, exhibit significant positive effects on withdrawal, while male gender (genderM) has a significant negative effect. Certain regions and educational backgrounds also influence withdrawal likelihood, with higher deprivation bands associated with increased withdrawal rates.

## Performance Metrics
Predictive model achieved an accuracy of approximately 70.28%, indicating that it correctly classified around 70.28% of all observations in the dataset. However, precision, recall, and the F1 score provide more subtle insights. The precision, measuring around 52.77%, indicates that approximately 52.77% of the observations predicted as positive by the model were actually positive. Recall, at approximately 17.00%, suggests that the model correctly identified only about 17.00% of all positive instances in the dataset. The F1 score, a balance between precision and recall, is approximately 25.71%, indicating a moderate overall performance.

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
The resampling results indicate that the model's predictions deviate from the actual values by an average RMSE of approximately 0.4457 units. The R-squared value is approximately 0.0818, suggesting that the model explains only about 8.18% of the variance in the dependent variable. The MAE is approximately 0.3969, indicating relatively close alignment between the model's predictions and the actual values. However, the low R-squared value implies that the model may not fully capture the variability in the data.

## Conclusion
While the predictive model demonstrates reasonable accuracy, precision, recall, and AUC metrics, there is room for improvement. The model's coefficients highlight significant predictors of withdrawal, providing actionable insights for intervention strategies. However, the model's explanatory power is limited, suggesting the need for further refinement through feature engineering, model selection, or parameter tuning. 


