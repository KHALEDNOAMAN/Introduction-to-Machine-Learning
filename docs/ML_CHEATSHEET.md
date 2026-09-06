# Machine Learning Cheatsheet

## Algorithm Selection
```
What is your goal?
|-- Predict a number? --> Regression
|   |-- Linear? --> Linear Regression
|   |-- Complex? --> Random Forest / XGBoost
|-- Predict a category? --> Classification
|   |-- Simple? --> Logistic Regression
|   |-- Best accuracy? --> Random Forest / XGBoost
|-- Find groups? --> Clustering
|   |-- Know K? --> K-Means
|   |-- Arbitrary shapes? --> DBSCAN
|-- Reduce dimensions? --> PCA / t-SNE / UMAP
```

## Key Metrics
| Task | Metric | When to Use |
|------|--------|------------|
| Regression | RMSE | General purpose |
| Regression | MAE | Robust to outliers |
| Classification | Accuracy | Balanced classes |
| Classification | F1-Score | Imbalanced classes |
| Classification | AUC-ROC | Ranking quality |

## Common Pitfalls
- Do NOT train on test data (data leakage)
- Do NOT ignore class imbalance
- Do NOT skip feature scaling for distance-based models
- Always use cross-validation
- Start simple, then add complexity