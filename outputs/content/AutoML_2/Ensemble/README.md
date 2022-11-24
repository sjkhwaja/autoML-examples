# Summary of Ensemble

[<< Go back](../README.md)


## Ensemble structure
| Model             |   Weight |
|:------------------|---------:|
| 3_Default_Xgboost |        5 |

## Metric details
|           |    score |     threshold |
|:----------|---------:|--------------:|
| logloss   | 0.267911 | nan           |
| auc       | 0.95594  | nan           |
| f1        | 0.901609 |   0.500049    |
| accuracy  | 0.891226 |   0.520298    |
| precision | 0.997674 |   0.995696    |
| recall    | 1        |   0.000343896 |
| mcc       | 0.780103 |   0.520298    |


## Metric details with threshold from accuracy metric
|           |    score |   threshold |
|:----------|---------:|------------:|
| logloss   | 0.267911 |  nan        |
| auc       | 0.95594  |  nan        |
| f1        | 0.901414 |    0.520298 |
| accuracy  | 0.891226 |    0.520298 |
| precision | 0.90123  |    0.520298 |
| recall    | 0.901599 |    0.520298 |
| mcc       | 0.780103 |    0.520298 |


## Confusion matrix (at threshold=0.520298)
|                  |   Predicted as long |   Predicted as short |
|:-----------------|--------------------:|---------------------:|
| Labeled as long  |                1742 |                  241 |
| Labeled as short |                 240 |                 2199 |

## Learning curves
![Learning curves](learning_curves.png)
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



[<< Go back](../README.md)
