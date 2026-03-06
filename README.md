# Amazon_Sales_data_Prediction

### 1️⃣ Time Series Analysis
- Total revenue in 2023 is slightly higher than in 2022, indicating steady growth.
- Monthly sales: **January** has the highest revenue, **February** the lowest.
- Quarterly sales: **Q3** has the highest revenue (~8,378,870.70), **Q4** the lowest (~8,107,577.80).

### 2️⃣ Exploratory Data Analysis (EDA)
- **Sales by Product:** Beauty products generate the highest revenue; Sports products generate the lowest.
- **Sales by Region:** Middle East contributes the most; Europe the least.
- **Payment Methods:** Wallet payments drive the highest sales, followed by UPI; debit card sales are lower.
- **Quantity Sold:** Books and Home & Kitchen products are sold in highest quantities.
- **Rating Impact:** Products rated 1.5–4.5 generate more revenue than 1.0 or 5.0.
- **Discount Percentage:** 0% discount products sell the most; 5% discount performs better than 10%; 30% discount results in very low revenue.

### 3️⃣ Correlation Analysis
- Total revenue is primarily driven by **price** and **quantity sold**.
- Discount percentage has a small negative effect.
- Rating and review count have negligible impact.

### 4️⃣ Linear Regression Observations
- **R² ≈ 0.87** → explains ~87% of variance in revenue.
- **RMSE ≈ 34k** → residual errors are relatively high; model is interpretable.
- Quantity sold is the most important factor driving revenue.
- Discounts reduce revenue slightly.
- Price has moderate effect.
- Other features are minor.
> **Actionable insight:** Focus on increasing units sold rather than over-discounting.

### 5️⃣ Random Forest Regression Observations
- **R² ≈ 0.99986** → almost perfect prediction.
- **RMSE ≈ 6** → extremely low error.
- **Feature Importance:** Price (0.52) → most important, Quantity Sold (0.45) → second most important.
- Other features (rating, review_count, category, region) are negligible.
> Revenue is largely determined by **price × quantity_sold**.

### 6️⃣ Overall Conclusion
1. **Revenue Drivers:** Price and quantity sold dominate; other features have minor impact.
2. **Sales Strategy Insights:** 
   - Focus on top-performing products (Beauty, Books, Home & Kitchen).
   - Use discounts carefully; high discounts do not always increase revenue.
   - Optimize payment methods (Wallet, UPI).
3. **Modeling Insights:** 
   - Linear Regression: interpretable feature impact.
   - Random Forest: highly accurate revenue predictions.
4. **Seasonality:** Peak months (January, Q3) should be targeted for marketing campaigns.
> **Key Recommendation:** Combine **demand forecasting** (Random Forest) with **feature impact analysis** (Linear Regression) to guide inventory, pricing, and promotions for maximizing Amazon revenue.

