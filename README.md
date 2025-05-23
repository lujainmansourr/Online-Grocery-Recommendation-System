# Online Grocery Product Reorder Prediction

A machine learning project aimed at predicting if customers will reorder grocery items based on their historical purchase data.

Created as part of an Introduction to Data Science course utilizing Python, Scikit-learn, and Jupyter Notebook.

## Project Summary

This project explores customer purchase histories to develop a classification model that forecasts reorder behavior for grocery products.

Three different algorithms were implemented and evaluated:

- K-Nearest Neighbors (KNN)  
- Decision Tree Classifier  
- Logistic Regression  

Model performance was assessed with key classification metrics to identify the most suitable approach.

## Highlights

- Combined user and product purchase datasets for comprehensive analysis  
- Performed feature engineering capturing behavioral insights  
- Compared model performance with accuracy, precision, recall, and ROC-AUC  
- Selected the optimal model balancing accuracy and prediction speed  

## Dataset Features Used

Main features utilized in model training:

- Total orders per user  
- Total products ordered by user  
- User reorder rate  
- Product popularity metrics  
- Position in cart (add_to_cart_order)  
- Order day of week and hour  
- Time since last order  

### Target Variable

- `reordered`: Binary indicator (1 if product reordered, else 0)  

## Model Evaluation Summary

| Model               | Accuracy | Precision | Recall | ROC-AUC |
|---------------------|----------|-----------|--------|---------|
| KNN (k=3)           | 0.66     | 0.70      | 0.76   | 0.69    |
| Decision Tree       | 0.66     | 0.71      | 0.71   | 0.65    |
| Logistic Regression | 0.66     | 0.70      | 0.75   | 0.70    |

**Final model choice:** Logistic Regression, due to its balanced metrics and computational efficiency.


## Technologies and Libraries

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Jupyter Notebook  
- Matplotlib / Seaborn (for optional data visualization)  

## Learning Outcomes

- Applying ML algorithms to real transactional data  
- Feature engineering for user-product interaction  
- Rigorous model evaluation and comparison  
- Conducting experiments interactively with Jupyter  

## Future Enhancements

- Explore ensemble techniques (Random Forest, Gradient Boosting)  
- Hyperparameter tuning via GridSearchCV or RandomizedSearchCV  
- Add richer user-product behavioral features  
- Deploy model as a REST API for integration with e-commerce platforms  

## License

This repository is intended for educational purposes only.

