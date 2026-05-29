#  Credit Risk & Loan Performance Dashboard
Credit Risk &amp; Loan Performance Dashboard built with Power BI | DAX | Power Query | BFSI Domain

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

- **42% unclassified risk categories** — A large portion of records had no risk classification. Instead of removing them, I retained these records and labeled them as 'Unknown' to preserve data completeness. In real banking systems, missing classifications are common due to legacy data migration issues.

- **Bankruptcy count ranged up to 5** — This is statistically unusual in real-world banking, where 4–5 bankruptcies per individual are extremely rare. This suggests the dataset may contain synthetic data — a common characteristic of public Kaggle datasets. In a production environment, I would validate this anomaly with the data engineering team before proceeding with analysis.

- **No date columns present** — The dataset contained no date columns, making time intelligence functions (YTD, MoM trends) inapplicable. Analysis was therefore focused on borrower segmentation and risk profiling rather than time-based trends.
---

## 🛠️ Tools & Technologies
- Power BI Desktop
- Power Query — data cleaning & transformation
- DAX — 11 custom measures

---

## 📁 Dataset
- Source: [Kaggle — Bank Loan Status Dataset](https://www.kaggle.com/datasets/zaurbegiev/my-dataset)
- Rows: ~89,000
- Domain: BFSI

## ❓ Problem Statement

Banks and NBFCs lose crores of rupees every year due to 
loan defaults (NPA — Non-Performing Assets). Traditional 
credit checks often rely on single factors like bankruptcy 
history, which this analysis proves is insufficient. 
This project analyzes 89,000+ loan records to identify 
patterns that better predict borrower default risk.

---

## 🎯 Objectives

1. Identify loan default patterns across borrower segments
2. Discover high-risk borrower profiles using multiple factors
3. Support data-driven loan approval decisions in banking

---

## 💡 Recommendations

Based on the analysis, banks should consider:

- Long-term loan applicants → stricter income verification 
  + higher interest rates
- Renters → lower loan amount approval + higher collateral 
  requirement
- High Risk borrowers → additional verification before 
  approval
- Avoid single-factor decisions — combine Credit Score, 
  DTI, Home Ownership & Loan Term
- Unknown risk category (42%) → treat as Medium Risk 
  until properly classified

---

## 🎨 Design Credits
- Icons: [Flaticon](https://flaticon.com) & [Icons8](https://icons8.com)
- Illustrations: [Storyset](https://storyset.com)

---

## 👤 Author
**Preethiv Ram** | Aspiring Data Analyst — BFSI Domain
[LinkedIn](https://www.linkedin.com/in/preethivram/) | [GitHub](https://github.com/preethivram-2k)
