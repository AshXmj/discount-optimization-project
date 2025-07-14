
# Discount Effectiveness Prediction

## 📄 Project Overview
This project focuses on predicting the effectiveness of discounts in driving sales and optimizing profitability. By analyzing historical sales data, it aims to help businesses identify optimal discount strategies and select eligible customers or items for targeted discounts.

## 💡 Problem Statement
Offering discounts is a common tactic to increase sales, but excessive or poorly targeted discounts can reduce overall profitability. This project builds predictive models to analyze discount impact and guide better discount decisions.

## 🗂️ Dataset
- **Source**: Proprietary sales dataset from a business partner (`Sales reportcsv.csv`)
- **Key features**: 
  - Bill No
  - BillDate
  - Name
  - Item
  - ItemHSN
  - TaxConfName
  - Mrp
  - Rate
  - LineDiscountPercent
  - LineSalesAccountVal
  - Quantity
  - ItemWiseDiscountsTotal
  - LineItemTax
## ⚙️ Methodology
- **Exploratory Data Analysis (EDA)**:
  - Checked data structure, types, and distributions
  - Identified missing values and basic patterns
- **Data preprocessing**: 
  - Handling missing values
  - Dropped duplicate records
  - Feature engineering on discount-related columns
  - Handled missing values using median imputation
  - Applied label encoding to categorical columns (`Name`, `Item`, `TaxConfName`)
  - Standardized numerical features using StandardScaler
- **Modeling**: 
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
  - Gradient Boosting Regressor
- **Evaluation metrics**: 
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - Root Mean Squared Error (RMSE)
  - R² score

## 📊 Results
- Regression models were trained and evaluated to predict profit outcomes based on discount strategies.
- Analysis indicated that offering an **optimal discount range of approximately 7.3%** maximizes profitability while avoiding unnecessary revenue loss.
- Feature importance analysis revealed that `LineDiscountPercent`, `LineSalesAccountVal`, and `ItemWiseDiscountsTotal` are key factors affecting profit.
- Visualizations demonstrated error distributions, model comparisons, and the effect of varying discount rates on predicted profit.
  
## ✅ Conclusion
This project demonstrates a data-driven approach to evaluating and optimizing discount strategies using regression modeling and detailed feature analysis. By identifying an optimal discount range of approximately 7.3%, the analysis helps maximize profitability without over-discounting. The combination of EDA, careful preprocessing, and multiple regression models allowed for a thorough understanding of how different features, especially discount percentage and sales value, impact overall profit. These findings provide actionable insights for businesses to design more effective discount campaigns, improve pricing strategies, and drive sustainable revenue growth.


## 💻 Tech Stack
- Python (Pandas, NumPy, Scikit-learn, Seaborn, Matplotlib)

## 🚀 Future Scope
- Integrating time-series sales forecasting
- Building an interactive dashboard for business users
- Including customer segmentation for personalized discounts

## 📬 Contact
Feel free to connect or reach out for any questions!
