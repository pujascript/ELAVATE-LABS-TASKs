# Task 1 - Data Cleaning: Mall_Customers Dataset

## Dataset Info
- **Rows**: 200
- **Columns**: 5 (`CustomerID`, `Gender`, `Age`, `Annual Income (k$)`, `Spending Score (1-100)`)

## Cleaning Steps
1. Standardized column names (snake_case).
2. Normalized Gender values to `Male`/`Female`.
3. Checked ranges:
   - Age between 10–100.
   - Annual income positive.
   - Spending score between 1–100.
4. Detected outliers in `Age` and `Annual Income` using IQR method.
   - Applied winsorization (capped extreme values).
5. Final cleaned dataset columns: `customer_id`, `gender`, `age`, `annual_income_k$`, `spending_score`.
```
