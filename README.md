# Bank Customer Churn Workbook Analysis

An Excel-based exploratory analysis of a 500-row bank-customer sample. The workbook contains descriptive pivot-table analysis, a two-sample salary t-test and a credit-score ANOVA.

## What is included

- Original input workbook preserved separately from the repaired analysis workbook
- Workbook verifier checks source-cell preservation and recomputes the reported ANOVA
- README summarizes the questions and key statistical results

## Run locally

```sh
python -m pip install -r requirements-analysis.txt
python scripts/verify_analysis.py
```

## Verify

The verifier checks the two workbooks, row/ID/missing-value conditions, and the stored F and p values. Open `Bank_Churn_Analysis_Repaired.xlsx` in Excel to inspect the sheets and charts.

## Repository map

`Bank+Churn+Data (version 1).xlsx` is the source workbook. `Bank_Churn_Analysis_Repaired.xlsx` contains the analysis. `scripts/verify_analysis.py` performs reproducibility checks.

## Evidence and limitations

The verifier checks 500 records and reproduces the workbook's three-group ANOVA (F ≈ 0.9898, p ≈ 0.3724). This validates workbook consistency, not the sampling process or a causal churn explanation.

The source and license of this 500-row sample are not documented. Some historical workbook questions use imputed values, and the original pre-imputation data is unavailable. Treat results as descriptive analysis, not a customer-retention policy or generalizable estimate.

## License

No repository license file is included. Unless the project owner adds a license, do not assume the code, data or model artifacts may be redistributed or reused. Verify third-party data and model terms separately.
