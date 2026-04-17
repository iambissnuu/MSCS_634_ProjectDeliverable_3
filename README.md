# MSCS 634 - Deliverable 3
## Classification, Clustering, and Pattern Mining

### Student Information
Name: Bishnu Sharma  
Course: MSCS 634  
Deliverable: Project Deliverable 3  
Date: 17 March, 2026  

---

## Project Description

This project applies advanced data mining techniques to the Bank Marketing dataset, including classification, clustering, and association rule mining. The goal is to predict customer subscription behavior, identify meaningful customer segments, and discover hidden patterns in the data to support data-driven decision-making.

---

## Dataset Description

The dataset contains customer demographic, financial, and campaign-related information collected from a banking institution. The target variable **y** indicates whether a customer subscribed to a term deposit.

---

## Techniques Used

### 1. Classification
- Models: Decision Tree, K-Nearest Neighbors (KNN)
- Hyperparameter Tuning: GridSearchCV (Decision Tree)
- Evaluation Metrics:
  - Accuracy
  - F1 Score
  - Confusion Matrix
  - ROC Curve

### 2. Clustering
- Model: K-Means Clustering
- Preprocessing: Feature scaling using StandardScaler
- Evaluation Metric:
  - Silhouette Score

### 3. Association Rule Mining
- Algorithm: Apriori
- Metrics:
  - Support
  - Confidence
  - Lift

---

## Key Findings

### Classification Insights
- The tuned Decision Tree model achieved the highest accuracy (~0.89), demonstrating that hyperparameter tuning significantly improves model performance.
- KNN showed lower F1 score, indicating difficulty in handling class imbalance and complex relationships in the dataset.

### Clustering Insights
- K-Means successfully segmented customers into distinct groups based on financial and behavioral characteristics.
- Some clusters represent high-value customers with higher balances, while others indicate lower engagement groups.
- These segments can be used for targeted marketing and customer retention strategies.

### Association Rule Insights
- Strong relationships were found between attributes such as job and education.
- High lift values indicate meaningful patterns that can help identify specific customer groups.
- These patterns can be used to design personalized marketing campaigns.

---

## Overall Insights

Each data mining technique contributes differently:
- Classification focuses on predicting customer behavior.
- Clustering helps identify natural customer segments.
- Association rule mining uncovers hidden relationships between variables.

By combining these approaches, the project provides a comprehensive understanding of the dataset, enabling better decision-making through prediction, segmentation, and pattern discovery.

---

## Challenges Encountered

- Handling categorical variables required one-hot encoding, which increased dataset dimensionality.
- Selecting optimal model parameters required experimentation and tuning.
- Clustering required proper feature scaling and interpretation of overlapping groups.
- Association rule mining required transforming data into transactional format and tuning support/confidence thresholds.

---

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- mlxtend

---

## Repository Contents

- `DataMining_Deliverable3.ipynb` → Main notebook with full implementation
- `bank-full.csv` → Dataset used for analysis
- `README.md` → Project summary and findings

---

## Conclusion

This project demonstrates how multiple data mining techniques can be applied together to extract meaningful insights from real-world data. The combination of classification, clustering, and pattern mining provides a comprehensive analytical framework for understanding customer behavior and improving business decision-making.
