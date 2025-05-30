# Sales Prediction using Machine Learning

## 📌 Project Overview
This project aims to predict product sales using machine learning techniques. Leveraging data about product properties and outlet characteristics, the goal is to help a retailer forecast sales performance more accurately to improve inventory planning and marketing strategies.

## 📊 Key Insights
1. **Outlet Size and Sales**: Medium-sized outlets were associated with the highest average sales, suggesting they may strike an optimal balance between foot traffic and operational efficiency.
   

2. **Product Type Influence**: Some product categories (like "Snack Foods" and "Dairy") consistently outperformed others in terms of sales, pointing to possible customer preference or seasonal demand effects.
   

## 🤖 Model Summary
A **Random Forest Regressor** was selected as the best-performing model after comparison with Linear Regression and hyperparameter tuning using GridSearchCV.

### 📈 Model Evaluation:
- **R² Score (Test Set)**: 0.72
- **Mean Absolute Error (MAE)**: 825.43
- **Root Mean Squared Error (RMSE)**: 1153.89

These metrics indicate that the model explains about 72% of the variance in sales and provides reasonably accurate predictions.

## 🗂️ Repository Contents
- `sales_prediction_model.ipynb`: Clean final notebook
- `images/`: Folder with key visualizations used above
- `README.md`: Summary and project report

## 🔍 Linear Regression Coefficients

![Linear Regression Coefficients](linear_regression_coefficients.png)

Top 3 impactful features:
- Item_MRP: Higher price = more sales
- Outlet_Type_Grocery Store: Lower sales in grocery stores
- Item_Visibility: Higher visibility = possibly lower sales

---

## 🌲 Random Forest Feature Importance

![Random Forest Feature Importances](random_forest_feature_importance.png)

Top 5 important features:
- Item_MRP
- Outlet_Type_Supermarket Type 1
- Outlet_Identifier_OUT027
- Item_Visibility
- Outlet_Establishment_Year

---

## ✅ Final Recommendation

The **tuned Random Forest model** performs best on test data and generalizes well.  
It captures both linear and non-linear relationships and shows consistent performance without overfitting.

We recommend deploying the Random Forest model to help guide product pricing, shelf visibility strategies, and store-type targeting.
