# Cleaning Log

Dataset: Sample Superstore (Kaggle)
Rows: 9,994

Steps (Power Query):
1. Imported the CSV with Get Data > From Text/CSV and promoted the first row to headers
2. Set Sales, Profit and Discount to Decimal Number; Quantity to Whole Number
3. Order Date and Ship Date arrived as text in US format (m/d/yyyy).
   Default conversion with Indian regional settings created blanks or swapped
   day and month. Re-converted using the English (United States) locale.
4. Verified in Column quality: 100% valid, 0% errors, 0% empty
5. Added columns in Excel: Year, Month Num, Month, Profit Margin
6. Verified PivotTable grand totals match the SUM formula: $2,297,200.86 sales,
   $286,397.02 profit, 5,009 unique orders
