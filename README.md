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
- Decision Tree performs better because it can capture nonlinear relationships between customer attributes.
- KNN showed a lower F1 score, indicating difficulty in handling class imbalance and complex decision boundaries.
- The lower F1 score highlights challenges in correctly identifying customers who subscribe to term deposits (minority class).

### Clustering Insights
- K-Means successfully segmented customers into three distinct groups based on financial and behavioral characteristics.
- For example, one cluster includes customers with higher balances (~2000+) and engagement, while another represents lower-value customers with less interaction.
- These segments can be used to design targeted marketing strategies, improve engagement, and enhance customer retention.

### Association Rule Insights
- Strong relationships were identified between customer attributes such as job and education.
- For example, the rule **(management → tertiary)** shows a high lift (~2.8), indicating a strong and meaningful relationship.
- These patterns can help identify specific customer groups and support personalized marketing campaigns.

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
- Selecting optimal model parameters required experimentation and hyperparameter tuning.
- Clustering required proper feature scaling and careful interpretation due to overlapping customer characteristics.
- Association rule mining required transforming data into transactional format and selecting appropriate support and confidence thresholds.

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

This project demonstrates how multiple data mining techniques can be applied together to extract meaningful insights from real-world data. The combination of classification, clustering, and association rule mining provides a comprehensive analytical framework for understanding customer behavior.

The results highlight how predictive modeling, customer segmentation, and pattern discovery can support targeted marketing, improve decision-making, and enhance overall business strategy.
