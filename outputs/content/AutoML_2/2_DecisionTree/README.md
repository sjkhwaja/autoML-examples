# Summary of 2_DecisionTree

[<< Go back](../README.md)


## Decision Tree
- **n_jobs**: -1
- **criterion**: gini
- **max_depth**: 3
- **explain_level**: 2

## Validation
 - **validation_type**: split
 - **train_ratio**: 0.75
 - **shuffle**: True
 - **stratify**: True

## Optimized metric
logloss

## Training time

16.6 seconds

## Metric details
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.454124 | nan         |
| auc       | 0.858947 | nan         |
| f1        | 0.825033 |   0.310846  |
| accuracy  | 0.792628 |   0.310846  |
| precision | 0.94211  |   0.841315  |
| recall    | 1        |   0.0420701 |
| mcc       | 0.581852 |   0.310846  |


## Metric details with threshold from accuracy metric
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.454124 |  nan        |
| auc       | 0.858947 |  nan        |
| f1        | 0.825033 |    0.310846 |
| accuracy  | 0.792628 |    0.310846 |
| precision | 0.771592 |    0.310846 |
| recall    | 0.886429 |    0.310846 |
| mcc       | 0.581852 |    0.310846 |


## Confusion matrix (at threshold=0.310846)
|                  |   Predicted as long |   Predicted as short |
|:-----------------|--------------------:|---------------------:|
| Labeled as long  |                1343 |                  640 |
| Labeled as short |                 277 |                 2162 |

## Learning curves
![Learning curves](learning_curves.png)

## Decision Tree 

### Tree #1
![Tree 1](learner_fold_0_tree.svg)

### Rules

if (Total Costs <= 8584.205) and (Total Costs <= 4865.995) and (CCS Diagnosis Code <= 253.5) then class: short (proba: 95.64%) | based on 3,278 samples

if (Total Costs <= 8584.205) and (Total Costs > 4865.995) and (CCS Diagnosis Code <= 454.5) then class: short (proba: 72.63%) | based on 2,769 samples

if (Total Costs > 8584.205) and (APR Severity of Illness Code <= 2.5) and (APR Medical Surgical Description > 0.5) then class: short (proba: 57.49%) | based on 1,868 samples

if (Total Costs > 8584.205) and (APR Severity of Illness Code <= 2.5) and (APR Medical Surgical Description <= 0.5) then class: long (proba: 75.53%) | based on 1,847 samples

if (Total Costs > 8584.205) and (APR Severity of Illness Code > 2.5) and (Total Costs > 15573.525) then class: long (proba: 95.33%) | based on 1,797 samples

if (Total Costs > 8584.205) and (APR Severity of Illness Code > 2.5) and (Total Costs <= 15573.525) then class: long (proba: 78.08%) | based on 958 samples

if (Total Costs <= 8584.205) and (Total Costs <= 4865.995) and (CCS Diagnosis Code > 253.5) then class: short (proba: 68.65%) | based on 453 samples

if (Total Costs <= 8584.205) and (Total Costs > 4865.995) and (CCS Diagnosis Code > 454.5) then class: long (proba: 86.44%) | based on 295 samples





## Permutation-based Importance
![Permutation-based Importance](permutation_importance.png)
## Confusion Matrix

![Confusion Matrix](confusion_matrix.png)


## Normalized Confusion Matrix

![Normalized Confusion Matrix](confusion_matrix_normalized.png)


## ROC Curve

![ROC Curve](roc_curve.png)


## Kolmogorov-Smirnov Statistic

![Kolmogorov-Smirnov Statistic](ks_statistic.png)


## Precision-Recall Curve

![Precision-Recall Curve](precision_recall_curve.png)


## Calibration Curve

![Calibration Curve](calibration_curve_curve.png)


## Cumulative Gains Curve

![Cumulative Gains Curve](cumulative_gains_curve.png)


## Lift Curve

![Lift Curve](lift_curve.png)



## SHAP Importance
![SHAP Importance](shap_importance.png)

## SHAP Dependence plots

### Dependence (Fold 1)
![SHAP Dependence from Fold 1](learner_fold_0_shap_dependence.png)

## SHAP Decision plots

### Top-10 Worst decisions for class 0 (Fold 1)
![SHAP worst decisions class 0 from Fold 1](learner_fold_0_shap_class_0_worst_decisions.png)
### Top-10 Best decisions for class 0 (Fold 1)
![SHAP best decisions class 0 from Fold 1](learner_fold_0_shap_class_0_best_decisions.png)
### Top-10 Worst decisions for class 1 (Fold 1)
![SHAP worst decisions class 1 from Fold 1](learner_fold_0_shap_class_1_worst_decisions.png)
### Top-10 Best decisions for class 1 (Fold 1)
![SHAP best decisions class 1 from Fold 1](learner_fold_0_shap_class_1_best_decisions.png)

[<< Go back](../README.md)
