# Customer Churn Analysis

A portfolio-ready practice project analyzing customer churn with **Python, pandas, Matplotlib, and SQL**. The project demonstrates data quality checks, handling missing values, KPI calculation, segmentation, visualizations, and SQL queries.

> **Transparency:** The CSV is synthetic data generated for practice. This is an independent learning project, not work completed for an employer and not real customer data.

## Business questions
- What percentage of customers churn?
- How does churn differ by contract type?
- Is churn different for newer and longer-tenure customers?
- How does churn vary by tech support status and payment method?
- What data quality checks should be performed before reporting?

## Folder structure
```text
customer_churn_analysis_project/
├── data/
│   └── customer_churn.csv
├── notebooks/
├── reports/
│   ├── figures/
│   ├── churn_by_contract.csv
│   ├── churn_by_payment_method.csv
│   ├── churn_by_tech_support.csv
│   ├── churn_by_tenure.csv
│   └── findings_summary.md
├── sql/
│   └── churn_analysis.sql
├── src/
│   └── analyze_churn.py
├── requirements.txt
├── .gitignore
└── README.md
```

## Tools
- Python 3.10+
- pandas
- Matplotlib
- SQL (SQLite-compatible queries)
- CSV

## Run the Python analysis
```bash
pip install -r requirements.txt
python src/analyze_churn.py
```
The script prints KPI results and regenerates summary CSVs and chart images in `reports/`.

## SQL practice
Open `sql/churn_analysis.sql`. Import `data/customer_churn.csv` into a SQL table named `customers`, then run the queries in a SQL client that supports SQLite syntax.

## Data dictionary
| Column | Description |
|---|---|
| CustomerID | Synthetic unique customer identifier |
| Gender, SeniorCitizen, Partner, Dependents | Basic customer attributes |
| TenureMonths | Number of months as a customer |
| PhoneService, InternetService | Service subscriptions |
| Contract | Contract duration |
| TechSupport | Whether tech support is subscribed |
| PaymentMethod | Payment method category |
| MonthlyCharges | Monthly service charge |
| TotalCharges | Approximate total charges |
| Churn | Whether the customer churned (`Yes`/`No`) |

## Example charts

### Churn by contract
![Churn by contract](reports/figures/churn_by_contract.png)

### Churn by tenure
![Churn by tenure](reports/figures/churn_by_tenure.png)

### Churn by tech support
![Churn by tech support](reports/figures/churn_by_tech_support.png)

## Limitations
- The dataset is synthetic and cannot support real business claims.
- Relationships are descriptive, not proof of causation.
- SQL queries are provided as practice material; Python output is generated separately.

## Portfolio presentation
Describe this as an independent customer churn analysis practice project. Add your own notes and improvements, and be ready to explain how missing values were handled, how churn rate was calculated, and what each chart shows.
