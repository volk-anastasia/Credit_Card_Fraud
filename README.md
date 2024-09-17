# Credit Card Fraud Detection
[Kaggle dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

**GOAL:** predict whether the transaction is fraud or not.  
**BEST SCORE:** 0.99 Accuracy (best model - DBSCAN)

---
## Architecture


#### EDA

The features:
1. Time - Number of seconds elapsed between this transaction and the first transaction in the dataset
2. V1-V28 - Result of a PCA Dimensionality reduction to protect user identities and sensitive features
3. Amount - Transaction amount
4. Class - 1 for fraudulent transactions, 0 otherwise

Dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions (492 of 284807).

![image](https://github.com/user-attachments/assets/c0ecfefd-a6d5-4cda-a323-2cdffe5854e2)


### Different models

**`Isolation Forest`**

Total metrics:
|                      |   Test   |
|----------------------|----------|
|            Accuracy: | 0.98     |
| Predicted anomalies: | 0.4266 % |

![image](https://github.com/user-attachments/assets/5a59751e-65fe-4158-92b2-efa3583c5129)


**`One-Class SVM`**

Total metrics:
|                      |   Test   |
|----------------------|----------|
|            Accuracy: | 0.98     |
| Predicted anomalies: | 0.4449 % |

![image](https://github.com/user-attachments/assets/4968e6bb-419b-472b-ab23-01b82d1bed6c)


**`Local Outlier Factor`**

Total metrics:
|                      |   Test   |
|----------------------|----------|
|            Accuracy: | 0.98     |
| Predicted anomalies: | 0.4252 % |

![image](https://github.com/user-attachments/assets/718fb99b-243c-4c87-8efc-8f168c49af0c)


**`DBSCAN`**

Total metrics:
|                      |   Test   |
|----------------------|----------|
|            Accuracy: | 0.99     |
| Predicted anomalies: | 0.2826 % |

![image](https://github.com/user-attachments/assets/d221699c-ad61-47a3-8591-e838274defee)

![image](https://github.com/user-attachments/assets/ae1cb804-71d8-4b83-83d3-d56e3be25793)
