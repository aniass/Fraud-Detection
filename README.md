# Fraud Detection

## General info

The project concerns the anomaly detection in credit cards transactions using machine learning models and Autoencoders. 
The main aim of this project is predict whether a given transaction was a fraud or not. The analysis includes data analysis, data preparation and creation model by using Isolation Forest, Local Outlier Factor, Support Vector Machine (OneClassSVM) algorithms and autoencoder model.

### Dataset

The dataset contains transactions made by credit cards in two days in 2013 by European cardholders and contains frauds as well. It comes from Kaggle and can be find [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## Motivation
The aim of this project is predict whether a given transaction was a fraud. The frauds in the credit cards industry are stealing or using stolen cards, or take more an aggressive form such as account takeover, counterfeiting and much more. The magnitude of credit card frauds is growing larger each day due to ever-increasing online transactions. Anomaly detection is an unsupervised data processing technique to detect anomalies from the dataset. Anomalies are data points that stand out amongst other data points in the dataset and do not fit the normal behavior in the data. These data points or observations deviate from the dataset’s normal behavioral patterns. The anomaly detection is very useful to detect fraud transactions just like in this case.

## Project contains:
- fraud detection using machine learning models - **Fraud_detection.ipynb**
- fraud detection using autoencoder model - **Fraud_Autoencoder.ipynb**

## Summary
The main aim of this project was prediction whether a given transaction was a fraud or not. The analysis included data analysis, data preparation and creation models by using Isolation Forest, Local Outlier Factor, Support Vector Machine (OneClassSVM) algorithms. In the first approach I evaluated our models with a few methods to check which model is the best. I used a accuracy score, f1 score, recall and confusion matrix. Finally the best model was One Class SVM with recall value 84%. That model has the lowest possible False Negatives rate and will be not miss many anomalies.

The second part of analysis I used autoencoders model to fraud anomaly detection. I built the model only on one-class examples (normal transactions) with no suspicious transactions. I evaluated our model with a few methods such as reconstruction error, recall and confusion matrix. The model captures 83% of the anomaly data points (based on recall value) and has the low False Negatives rate and will be not miss many anomalies.

## Technologies

The project is created with:
- Python 3.9
- libraries: tensorflow, pandas, numpy, scikit-learn, seaborn, matplotlib.

**Running the project:**

To run this project use Jupyter Notebook or Google Colab.

### References:
- [Anomaly detection algorithms](https://towardsdatascience.com/5-anomaly-detection-algorithms-every-data-scientist-should-know-b36c3605ea16)
- [Credit card fraud detection using autoencoders](https://medium.com/@curiousily/credit-card-fraud-detection-using-autoencoders-in-keras-tensorflow-for-hackers-part-vii-20e0c85301bd)
- [Complete guide to anomaly detection with autoencoders](https://www.analyticsvidhya.com/blog/2022/01/complete-guide-to-anomaly-detection-with-autoencoders-using-tensorflow/)

