# 📐 Underwriting & Credit Risk Scoring Methodology

## **Mathematical Framework & Regulatory Credit Appraisal Architecture**

---

## 1. The 100-Point Financial-Statement-Driven RAM Scorecard

The platform employs a deterministic 100-point credit risk model calibrated exclusively on audited financial statements, solvency metrics, and fundamental business efficiency.

```
Total RAM Score = [ Financial Performance (60 pts) ] + [ Capital Structure & Solvency (25 pts) ] + [ Business Fundamentals (15 pts) ]
```

---

### Category 1: Financial Performance & Cash Flow (60 Points Max)

| Parameter | Formula / Basis | Max Points | Optimal Benchmark | Risk Deduction Logic |
| :--- | :--- | :---: | :--- | :--- |
| **Current Ratio (CR)** | $\text{Current Assets} / \text{Current Liabilities}$ | **10 pts** | $\ge 1.33$ | $1.20 - 1.33 \rightarrow 7\text{ pts}$, $1.00 - 1.20 \rightarrow 4\text{ pts}$, $< 1.00 \rightarrow 0\text{ pts}$ |
| **Debt Service Coverage Ratio (DSCR)** | $\frac{\text{PAT} + \text{Deprec.} + \text{Interest}}{\text{Principal Repayment} + \text{Interest}}$ | **10 pts** | $\ge 1.75$ | $1.50 - 1.75 \rightarrow 8\text{ pts}$, $1.20 - 1.50 \rightarrow 5\text{ pts}$, $< 1.20 \rightarrow 0\text{ pts}$ |
| **Operating Profit Margin (OPM)** | $\text{EBITDA} / \text{Revenue} \times 100$ | **10 pts** | $\ge 15\%$ | $10\% - 15\% \rightarrow 7\text{ pts}$, $5\% - 10\% \rightarrow 4\text{ pts}$, $< 5\% \rightarrow 0\text{ pts}$ |
| **Interest Service Coverage (ISCR)** | $\text{EBIT} / \text{Interest Expense}$ | **10 pts** | $\ge 3.0$ | $2.0 - 3.0 \rightarrow 7\text{ pts}$, $1.5 - 2.0 \rightarrow 4\text{ pts}$, $< 1.5 \rightarrow 0\text{ pts}$ |
| **Revenue Growth & 3Y CAGR** | $(\text{Rev}_{FY} - \text{Rev}_{FY-1}) / \text{Rev}_{FY-1}$ | **8 pts** | $\ge 15\%$ | $8\% - 15\% \rightarrow 5\text{ pts}$, $0\% - 8\% \rightarrow 3\text{ pts}$, Negative $\rightarrow 0\text{ pts}$ |
| **Return on Capital Employed (ROCE)** | $\text{EBIT} / (\text{Total Assets} - \text{Current Liabilities})$ | **7 pts** | $\ge 18\%$ | $12\% - 18\% \rightarrow 5\text{ pts}$, $8\% - 12\% \rightarrow 3\text{ pts}$, $< 8\% \rightarrow 0\text{ pts}$ |
| **CFO to Total Debt** | $\text{Cash Flow from Operations} / \text{Total Debt}$ | **5 pts** | $\ge 25\%$ | $15\% - 25\% \rightarrow 3\text{ pts}$, $< 15\% \rightarrow 0\text{ pts}$ |

---

### Category 2: Capital Structure & Solvency (25 Points Max)

| Parameter | Formula / Basis | Max Points | Optimal Benchmark | Risk Deduction Logic |
| :--- | :--- | :---: | :--- | :--- |
| **TOL / ATNW** | $\text{Total Outside Liabilities} / \text{Adjusted Tangible Net Worth}$ | **10 pts** | $\le 2.50$ | $2.50 - 3.50 \rightarrow 7\text{ pts}$, $3.50 - 4.50 \rightarrow 3\text{ pts}$, $> 4.50 \rightarrow 0\text{ pts}$ |
| **Debt to Equity Ratio** | $\text{Total Long-Term Debt} / \text{Tangible Net Worth}$ | **6 pts** | $\le 1.50$ | $1.50 - 2.50 \rightarrow 4\text{ pts}$, $> 2.50 \rightarrow 0\text{ pts}$ |
| **Net Worth Buffer** | Absolute Tangible Net Worth (ATNW) | **5 pts** | $\ge ₹10\text{ Cr}$ | $₹5\text{Cr} - ₹10\text{Cr} \rightarrow 3\text{ pts}$, $< ₹5\text{Cr} \rightarrow 1\text{ pt}$ |
| **Debt to EBITDA Multiple** | $\text{Total Debt} / \text{EBITDA}$ | **4 pts** | $\le 3.0\times$ | $3.0\times - 4.5\times \rightarrow 2\text{ pts}$, $> 4.5\times \rightarrow 0\text{ pts}$ |

---

### Category 3: Business Fundamentals & Operating Efficiency (15 Points Max)

| Parameter | Formula / Basis | Max Points | Optimal Benchmark | Risk Deduction Logic |
| :--- | :--- | :---: | :--- | :--- |
| **Debtor Collection Days** | $(\text{Trade Receivables} / \text{Revenue}) \times 365$ | **5 pts** | $\le 60\text{ Days}$ | $60 - 90\text{ Days} \rightarrow 3\text{ pts}$, $> 90\text{ Days} \rightarrow 0\text{ pts}$ |
| **Inventory Holding Days** | $(\text{Inventory} / \text{COGS}) \times 365$ | **4 pts** | $\le 60\text{ Days}$ | $60 - 90\text{ Days} \rightarrow 2\text{ pts}$, $> 90\text{ Days} \rightarrow 0\text{ pts}$ |
| **Fixed Asset Turnover** | $\text{Revenue} / \text{Net Fixed Assets}$ | **3 pts** | $\ge 4.0\times$ | $2.5\times - 4.0\times \rightarrow 2\text{ pts}$, $< 2.5\times \rightarrow 0\text{ pts}$ |
| **Operating Cycle Efficiency** | $\text{Debtor Days} + \text{Inventory Days} - \text{Payable Days}$ | **3 pts** | $\le 90\text{ Days}$ | $90 - 120\text{ Days} \rightarrow 2\text{ pts}$, $> 120\text{ Days} \rightarrow 0\text{ pts}$ |

---

## 2. RAM Risk Grade Classification & Underwriting Directives

| Score Range | RAM Risk Grade | Risk Profile | Underwriting Decision & Covenants |
| :---: | :--- | :--- | :--- |
| **80 – 100** | **RAM-1** | Minimal Risk / Prime | **Recommended for Approval**. Eligible for prime lending rates; standard security covenants. |
| **65 – 79** | **RAM-2** | Low to Moderate Risk | **Recommended for Approval**. Standard pricing; quarterly compliance monitoring. |
| **50 – 64** | **RAM-3** | Moderate Risk | **Conditional Approval**. Minimum 100% SARFAESI collateral cover; personal promoter guarantee required. |
| **35 – 49** | **RAM-4** | High Risk | **Credit Committee Escalation**. Requires additional collateral cover ($\ge 125\%$) and monthly drawing power audits. |
| **< 35** | **RAM-5** | Critical Risk | **Decline / Ineligible**. Fundamental financial weakness or excessive leverage. |

---

## 3. Working Capital & MPBF Engine (Tandon Method II)

The platform evaluates the **Maximum Permissible Bank Finance (MPBF)** according to Reserve Bank of India (RBI) Tandon Committee guidelines:

$$\text{Working Capital Gap (WCG)} = \text{Total Current Assets (TCA)} - \text{Other Current Liabilities (OCL)}$$

$$\text{Minimum Stipulated Net Working Capital (NWC)} = 0.25 \times \text{Total Current Assets (TCA)}$$

$$\text{MPBF (Method II)} = \text{WCG} - \text{Stipulated NWC} = \text{WCG} - (0.25 \times \text{TCA})$$

$$\text{Assessed Bank Finance} = \min(\text{MPBF Method II}, \text{Borrower Requested Facility})$$

---

## 4. Intelligent Schedule Completeness & Fallback Engine

Audited financial reports often arrive with missing schedule annexures (e.g., Debtor Aging Schedule or Inventory Breakdown). Instead of rejecting the application or stalling the underwriter, the engine:

1. **Detects Missing Schedules:** Automatically identifies whether Debtor Schedule, Inventory Schedule, or Fixed Asset Schedule are attached.
2. **Activates Mathematical Fallback:** Derives debtor velocity from aggregate Balance Sheet trade receivables and revenue.
3. **Contextual Flagging:** Generates a highlighted recommendation inside the Credit Appraisal Memo (CAM) requesting the underwriter obtain the schedule prior to final loan disbursement.
