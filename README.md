# datainsightx

`datainsightx` is a lightweight Python package that generates automated summaries and visual reports from transactional datasets. It's designed to help analysts and stakeholders quickly understand key patterns in their data — with minimal setup.

The tool detects useful columns, calculates relevant KPIs, creates visualizations, and saves the outputs as plain text, JSON, and HTML files.

---

## What it does

Given a basic CSV file with a date column and a numeric value column (optionally a category column), `datainsightx`:

- Automatically identifies key columns (date, value, and category)
- Computes important metrics such as total, monthly average, month-over-month change, and year-over-year growth
- Highlights top categories based on value
- Creates visual charts for trends and category distribution
- Exports:
  - A text summary
  - A structured JSON report
  - A full HTML report with embedded visualizations

---

## How to use

1. Place your CSV file in the working directory.
2. Call the `run_insight()` function with the CSV file path.

```python
from core import run_insight

run_insight("your_file.csv")
