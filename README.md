# Bank Customer Churn Workbook Analysis

An Excel-based analysis of a 500-row bank customer dataset. The workbooks organize descriptive comparisons of customer attributes, a two-sample t-test for salary, and an ANOVA for credit score across churn groups.

`Bank+Churn+Data (version 1).xlsx` is preserved as the source workbook. `Bank_Churn_Analysis_Repaired.xlsx` contains the repaired analysis, pivot tables, and charts. `scripts/verify_analysis.py` checks the record and ID conditions, source-cell preservation, and recomputes the reported ANOVA (F about 0.9898, p about 0.3724).

## Reproduce the checks

```sh
python -m pip install -r requirements-analysis.txt
python scripts/verify_analysis.py
```

Open the repaired workbook in Excel to inspect the sheets and visual summaries.
