# Predicting Plant Health Using Machine Learning

## Overview  
This application predicts the health status of plants using a machine learning classifier. The dataset contains information about various environmental and biological factors that influence plant health. The goal is to build an accurate predictive model to assist in early detection and classification of plant health issues.

The dataset used is synthetically generated or collected from agricultural sources containing labeled records of healthy and unhealthy plant instances.

---
## Media

<img src="images/outputTree.pdf" width="500" alt="Decision Tree Diagram"/>
<em>Visual of trained decision tree classifier (interpretable logic)</em></p>

<img src="images/automation-slides.pdf" width="500" alt="Automation Slides"/>
<em>Visual all of our "Why AI?" slides</em></p>

---

## Understanding the Data  
In agriculture, early and accurate identification of plant health conditions is crucial to prevent crop loss and optimize yield. Factors influencing plant health include temperature, humidity, light intensity, soil conditions, and visible symptoms like discoloration or spots. Correctly identifying and leveraging these features can lead to timely interventions, improving agricultural productivity and resource efficiency.

---

## Data Understanding  
This dataset includes multiple features such as environmental conditions (temperature, humidity), soil properties, and categorical observations (e.g., leaf color, plant type). The target variable is the **plant health status**, typically labeled as "healthy", "infected", or "needs attention". 

Each data point represents a single observation of a plant under certain conditions.

---

## Understanding Task  
The objective is to build a predictive machine learning model that classifies plant health status based on given features. The model is trained to understand patterns and correlations between features and the health outcome.

---

## Modeling  
A **Random Forest Classifier** is used to model the data. The following steps were performed:

- Data cleaning and preprocessing  
- Encoding of categorical variables using One-Hot Encoding  
- Feature scaling of numerical attributes  
- Train-test split for model validation  
- Model training using Random Forest  
- Performance evaluation with classification metrics  
- Confusion matrix visualization  
- Model artifacts (model, encoder, scaler) were saved for future use

---

## Evaluation  
The trained model is evaluated based on the following metrics:

- **Accuracy Score**: Measures overall correctness  
- **Precision**: Useful for minimizing false positives  
- **Recall**: Useful for identifying all true positives (especially critical in early disease detection)  
- **F1 Score**: Balances precision and recall  
- **Confusion Matrix**: Visualizes correct vs incorrect predictions  

The model achieved high accuracy and balanced precision-recall performance, indicating it is a strong candidate for field use.

---

## Findings  

- The Random Forest Classifier showed strong performance across all evaluation metrics.  
- Environmental features such as temperature and humidity had high importance in predicting plant health.  
- One-Hot Encoding of categorical features like plant type and leaf color improved model interpretability.  
- Early signs of disease or poor health were detectable from subtle feature differences.

---

## Next Steps and Recommendations  

- Further improvements can be achieved by exploring ensemble methods like Gradient Boosting or XGBoost.  
- Model can be fine-tuned further based on business needs (e.g., maximizing recall to avoid missing sick plants).  
- Deploy model on cloud-based agricultural platforms for real-time predictions.  
- Integrate drone/sensor imagery data for richer features.  
- Additional visualizations and SHAP-based interpretability can enhance trust in predictions.  
