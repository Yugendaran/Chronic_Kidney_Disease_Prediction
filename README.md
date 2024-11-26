# INNOVATIVE MACHINE LEARNING STRATEGIES FOR EARLY CHRONIC KIDNEY DISEASE PREDICTION: LEVERAGING CLINICAL DATA
The project output screenshots are shown as follows:
 

## Classification report
The presented output demonstrates the classification performance of two machine learning algorithms—Extra Trees and XGBoost—used for predicting Chronic Kidney Disease (CKD) based on clinical biomarkers. The classification reports provide insights into the models' precision, recall, F1-score, and accuracy metrics, evaluated on two classes: 0 (non-CKD) and 1 (CKD). These metrics are crucial for assessing the effectiveness of the models in distinguishing between CKD and non-CKD patients.

### Classification Report For Extra Tree and XGBoost :
![image](https://github.com/user-attachments/assets/c2d8ad2c-f29f-44d8-a85d-bb00f661f3e8)




### Extra Trees:
For the Extra Trees classifier, the accuracy achieved is 99%, which reflects the model's robustness in predicting CKD outcomes. The precision, recall, and F1-scores for both classes are nearly perfect, with scores of 0.97-1.00 across the board. This indicates that the model is highly effective in minimizing both false positives and false negatives. The macro and weighted averages for all metrics are consistently at 0.99, signifying balanced performance across both classes regardless of the class distribution.
### XGBoost:
The XGBoost classifier exhibits an accuracy of 98%, which is slightly lower than Extra Trees but still represents excellent predictive performance. The precision, recall, and F1-scores for class 0 are 0.95, 1.00, and 0.97, respectively, while for class 1, they are 1.00, 0.97, and 0.98. This suggests that XGBoost is highly effective in detecting CKD cases but slightly less precise in distinguishing non-CKD cases compared to Extra Trees. The macro and weighted averages remain consistently high at 0.97-0.98, indicating strong performance.


## Confusion Matrix For Extra Tree and XGBoost
The confusion matrices for the Extra Trees and XGBoost classifiers illustrate their performance in distinguishing between Chronic Kidney Disease (CKD) and non-CKD cases. Each matrix contains the counts of correctly and incorrectly classified instances for two classes: "No CKD" and "CKD."

 
### Confusion Matrix :
![image](https://github.com/user-attachments/assets/8013fada-e413-45e1-b7be-32f2e6bf18de)

### Extra Trees Classifier:
The confusion matrix for the Extra Trees model shows excellent predictive performance. Out of 72 actual "No CKD" cases, the model correctly identified 71 and misclassified only 1. For the "CKD" class, the model correctly classified 126 out of 128 cases and made 2 errors. These results highlight the model's ability to accurately predict both classes, with minimal misclassification, ensuring reliable predictions in a clinical setting.

### XGBoost Classifier:
The confusion matrix for the XGBoost model also demonstrates strong performance, though slightly less accurate than Extra Trees. All 72 "No CKD" cases were classified correctly, resulting in no false positives. For the "CKD" class, the model correctly identified 124 cases out of 128, with 4 misclassifications. While the accuracy is slightly lower than Extra Trees, the model still performs well in predicting CKD and non-CKD cases.

## Performance Metrics Comparison Of Machine Learning Model 
The heatmap provides a comparative analysis of various machine learning models based on four key performance metrics: accuracy, precision, recall, and F1-score, for predicting Chronic Kidney Disease (CKD). 
 
### Overall comparsion of Machine Learning Models 
![image](https://github.com/user-attachments/assets/483da8da-708b-4485-b60b-ffcf9f79aba1)


Among the models, Extra Trees outperforms others with near-perfect scores of 99% across all metrics, showcasing its exceptional ability to handle feature interactions and noisy data effectively. XGBoost and LightGBM also demonstrate strong performance, achieving accuracies of 98% and 97%, respectively, with balanced precision and recall, making them reliable alternatives for CKD prediction. Multi-Layer Perceptron (MLP) achieves a respectable 96% accuracy, while simpler models like KNN and Gaussian Naive Bayes lag behind with accuracies of 92% and 93%, respectively, indicating their limitations in capturing complex relationships in the dataset. Overall, the analysis highlights the superiority of ensemble learning methods, particularly Extra Trees, for early and accurate CKD prediction using clinical biomarkers.
  

## Integration of Machine Learning Models For Chronic Kidney Disease Prediction. 
The integration of machine learning models for Chronic Kidney Disease (CKD) prediction involves leveraging diverse algorithms to enhance diagnostic accuracy, robustness, and reliability. CKD, being a progressive condition, requires early detection and precise evaluation based on clinical biomarkers such as blood pressure, serum creatinine, and proteinuria levels. By integrating machine learning models, we aim to process this complex and high-dimensional data efficiently, ensuring accurate predictions and reducing the chances of misdiagnosis. 
![image](https://github.com/user-attachments/assets/405ad913-d332-4b17-b16e-d157a8b8c52f)




In this approach, different models are combined to utilize their unique strengths. Ensemble methods like Random Forest and Extra Trees provide robust predictions by aggregating decisions from multiple trees, ensuring high accuracy and reduced sensitivity to noisy data. Advanced boosting algorithms like XGBoost and LightGBM further enhance prediction by iteratively minimizing errors, achieving superior precision and recall. On the other hand, traditional models such as Logistic Regression offer interpretability, helping clinicians understand the influence of individual biomarkers on CKD progression. Additionally, neural networks like Multi-Layer Perceptron (MLP) capture non-linear patterns within the data, making them valuable for handling complex biomarker interactions.
The integration may also involve stacking models, where predictions from base models (e.g., Random Forest, XGBoost) serve as inputs for a meta-model, further refining the results. This hybrid methodology ensures a balance between model interpretability, computational efficiency, and prediction accuracy. Through such integration, the system not only predicts CKD at an early stage but also provides actionable insights, aiding in personalized treatment planning and effective resource allocation in healthcare settings. This holistic approach addresses the limitations of individual models and maximizes the utility of machine learning in CKD prediction.
