# credit-risk-loan-performance-dashboard
Credit Risk &amp; Loan Performance Dashboard built with Power BI | DAX | Power Query | BFSI Domain

# Credit Risk & Loan Performance Dashboard
### Power BI | DAX | Power Query | BFSI Domain

---

## 📌 Project Overview
An interactive 3-page Power BI dashboard analyzing 89,000+ loan records to uncover credit risk patterns, borrower behavior, and loan performance in the BFSI domain.

---

## 📊 Dashboard Pages
| Page | Description |
|------|-------------|
| Summary | KPIs, Loan Status Distribution, Loans by Purpose, Term & Home Ownership |
| Risk Analysis | Default Rate by Risk Category, Home Ownership, Loan Term, Employment Length & Bankruptcy |
| Details (Drill-through) | Loan-level table — Loan ID, Status, Amount, Credit Score, Risk Category, Loan Size |

---

## 🧮 DAX Measures (11 Custom Measures)
| Measure | Purpose |
|---------|---------|
| Total Loans | Count of all loan records |
| Total Funded Amount | Sum of all funded loan amounts |
| Charged Off Loans | Count of defaulted loans |
| Charged Off Rate % | % of loans that defaulted |
| Full Paid Loans | Count of fully repaid loans |
| Avg Credit Score | Average borrower credit score |
| Avg Annual Income | Average borrower annual income |
| Avg Monthly Debt | Average monthly debt per borrower |
| Debt to Income Ratio | DTI % across borrowers |
| Long Term Loans | Count of 60-month loans |
| Short Term Loans | Count of 36-month loans |

---

## 🗂️ Data Model
- Fact table: `Loan_Data` (~89K rows)
- Dimension table: `dim_loan_status`
- Relationship: Loan_Status column

---

## 🔍 Key Insights
- Charged-Off Rate: **25.6%** — 1 in 4 loans defaulted
- Long-term loans: **32.8%** default vs **22.6%** short-term
- Renters default more (**28.3%**) than Home Mortgage holders (**23.2%**)
- High Risk: **31.8%** default vs Low Risk: **5.8%**
- Avg Credit Score: **715** | Avg DTI: **16%**
- Borrowers with zero bankruptcy history defaulted at **25.7%** — suggesting bankruptcy count alone is not a reliable default predictor

---

## ⚠️ Data Quality Findings
- 42% unclassified risk categories — reflects missing data in legacy banking systems
- Bankruptcy count up to 5 — statistically rare in real-world; likely synthetic Kaggle dataset
- No date columns — time intelligence not applicable; analysis focused on borrower segmentation

---

## 🛠️ Tools & Technologies
- Power BI Desktop
- Power Query — data cleaning & transformation
- DAX — 11 custom measures

---

## 📁 Dataset
- Source: Kaggle — Bank Loan Status Dataset
- Rows: ~89,000
- Domain: BFSI

---

## 🎨 Design Credits
- Icons: [Flaticon](https://flaticon.com) & [Icons8](https://icons8.com)
- Illustrations: [Storyset](https://storyset.com)

---

## 👤 Author
**Preethiv** | Aspiring Data Analyst — BFSI Domain
[LinkedIn](#) | [GitHub](#)
