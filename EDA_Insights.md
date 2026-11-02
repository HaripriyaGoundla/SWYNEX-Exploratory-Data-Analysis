# EDA Summary – SWYNEX Task 2

1. Dataset contains 10 rows and 8 columns.
2. 7 of 10 customers are active (70.0%); 3 are inactive (30.0%).
3. United States is the most represented country with 2 customers; each other named country has 1 customer. One country value is missing.
4. Among 9 valid signup dates, 7 customers signed up in January 2026 (77.8%); May and October each have 1 signup.
5. Amount has 9 non-missing values: mean 1,657.83, median 1,200.00, min -30.00, max 5,000.00. Mean exceeds median, influenced by high values.
6. One record has a negative amount (-30.00), flagged by negative_amount=True; validate whether it represents a refund, adjustment, or data error.
7. Missing values: Full Name, signup date, amount, and country each have 1 missing value (10% of rows for each).
8. Maximum amount is 5,000.00 for the United Kingdom record; inspect it as a potential high-value observation, not automatically an error.

## Interpretation
The sample is small (10 records). Treat findings as descriptive. Confirm the meaning of negative amounts and investigate missing values and the 5,000 amount before making business decisions.
