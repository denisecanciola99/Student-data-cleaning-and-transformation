Datasets for practicing data manipulation (cleaning + transformation)

1) retail_sales_raw.csv
   - Problems: mixed currency formats, discount as %, blanks/NA, invalid emails, duplicates
   - Try: parse dates, convert money columns to numeric, standardize discount to decimal, dedupe by order_id, validate email

2) student_term_raw.csv
   - Problems: inconsistent term formats, GPA/balance as strings, holds_count non-numeric, duplicates/conflicts (units_earned=99)
   - Try: normalize term to YYYYFA/YYYYSP, coerce numeric cols, fix/flag impossible values, create retention rate by major

3) cash_transactions_raw.csv
   - Problems: datetime formats, negative amounts w/ parentheses, missing references, duplicates with different statuses
   - Try: parse datetime, clean amount to numeric, compute daily net, reconcile reversals, flag pending > 7 days

Suggested outputs:
- Create cleaned versions: *_clean.csv
- Create summary tables: e.g., retention_by_major.csv, sales_kpis_by_store_month.csv, daily_net_cash.csv
