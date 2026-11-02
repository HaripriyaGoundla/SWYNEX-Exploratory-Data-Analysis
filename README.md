# SWYNEX – Exploratory Data Analysis (Task 2)

## Objective
Explore the cleaned customer dataset from Task 1 using Python, summarize key statistics, visualize patterns, and flag potential anomalies.

## Dataset
- Rows: 10
- Columns: 8
- File: `cleaned_customer_data.csv`

## Tools
Python, pandas, matplotlib, Jupyter Notebook.

## Key findings
- Dataset contains 10 rows and 8 columns.
- 7 of 10 customers are active (70.0%); 3 are inactive (30.0%).
- United States is the most represented country with 2 customers; each other named country has 1 customer. One country value is missing.
- Among 9 valid signup dates, 7 customers signed up in January 2026 (77.8%); May and October each have 1 signup.
- Amount has 9 non-missing values: mean 1,657.83, median 1,200.00, min -30.00, max 5,000.00. Mean exceeds median, influenced by high values.
- One record has a negative amount (-30.00), flagged by negative_amount=True; validate whether it represents a refund, adjustment, or data error.
- Missing values: Full Name, signup date, amount, and country each have 1 missing value (10% of rows for each).
- Maximum amount is 5,000.00 for the United Kingdom record; inspect it as a potential high-value observation, not automatically an error.

## Visualizations
- `charts/customers_by_country.png`
- `charts/customer_activity.png`
- `charts/amount_distribution.png`
- `charts/signups_by_month.png`

## How to run
1. Install Python, Jupyter, pandas and matplotlib.
2. Keep `cleaned_customer_data.csv` in the same folder as the notebook.
3. Open `SWYNEX_Exploratory_Data_Analysis.ipynb` and run all cells.

## Limitation
The dataset contains only 10 records. Results are descriptive and should not be generalized to a larger customer population without more data.
