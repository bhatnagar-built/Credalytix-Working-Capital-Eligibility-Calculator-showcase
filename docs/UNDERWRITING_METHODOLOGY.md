# 📐 Underwriting & Credit Risk Scoring Framework

## **Institutional Commercial Credit Appraisal Architecture**

> [!IMPORTANT]
> **Confidential & Proprietary Framework**  
> Exact mathematical weights, proprietary multi-factor ratio deduction algorithms, scoring thresholds, and calibrated risk rubrics are confidential intellectual property. This document provides a high-level overview of the underwriting dimensions evaluated by the engine.

---

## 1. Credit Risk Assessment Model (RAM) Architecture

The platform evaluates commercial borrowers across three core quantitative pillars derived from multi-year audited financial statements:

```
Total Credit Assessment = [ Pillar 1: Financial Performance & Cash Flow ] 
                         + [ Pillar 2: Capital Structure & Solvency ] 
                         + [ Pillar 3: Business Fundamentals & Operating Efficiency ]
```

---

### Pillar 1: Financial Performance & Cash Flow
*Focuses on operational profitability, debt servicing adequacy, and cash generation capability.*

- **Liquidity Health:** Multi-tier liquidity assessment evaluating short-term obligation coverage and buffer against working capital shocks.
- **Debt Service Capability:** Comprehensive coverage analysis evaluating operating cash flows against principal amortization and interest service liabilities.
- **Operating Profitability & Margins:** Trend analysis of operating profit margins (EBITDA), revenue quality, and gross profitability.
- **Revenue Trajectory & Growth:** Multi-year compound annual growth rate (CAGR) and year-on-year expansion velocity.
- **Capital Return Efficiency:** Assessment of return on capital employed (ROCE) and asset efficiency.
- **Operating Cash Flow Quality:** Quality of earnings assessment comparing cash flow from operations (CFO) against total financial debt.

---

### Pillar 2: Capital Structure & Solvency
*Focuses on balance sheet leverage, capital adequacy, and long-term financial stability.*

- **Leverage Multiples:** Comprehensive assessment of outside liabilities relative to adjusted tangible net worth (ATNW).
- **Gearing & Debt-to-Equity:** Evaluation of long-term debt burden relative to owner capital and equity cushions.
- **Capital Buffer & Net Worth Strength:** Absolute tangible capital size and capacity to absorb unexpected market shocks.
- **Debt-to-Operating Earnings:** Multiple of total debt obligations relative to annualized operating EBITDA.

---

### Pillar 3: Business Fundamentals & Operating Efficiency
*Focuses on working capital management, cash conversion cycle, and asset utilization.*

- **Debtor Velocity & Collection Efficiency:** Assessment of receivables velocity, collection cycles, and customer concentration risk.
- **Inventory Turnover & Holding Efficiency:** Evaluation of inventory days relative to industry operating norms.
- **Fixed Asset Productivity:** Operating revenue generated per unit of net fixed productive assets.
- **Operating Cash Cycle:** Net working capital cycle duration from raw material procurement to cash realization.

---

## 2. Risk Grading & Underwriting Directives

The engine maps borrowers into standard institutional credit risk tiers with automated policy recommendations:

| Risk Classification | Risk Profile | Underwriting Action |
| :---: | :--- | :--- |
| **Tier 1 (Prime)** | Superior financial health, strong solvency, and robust cash flows. | **Recommended for Approval**. Eligible for prime lending rates and standard security covenants. |
| **Tier 2 (Good)** | Healthy financial ratios with manageable debt levels. | **Recommended for Approval**. Standard pricing with periodic covenant monitoring. |
| **Tier 3 (Moderate)** | Acceptable credit profile with moderate leverage. | **Conditional Approval**. Enhanced collateralization and promoter guarantees stipulated. |
| **Tier 4 (Elevated Risk)**| Financial stretch or high leverage detected. | **Credit Committee Escalation**. Requires additional security cover and enhanced monitoring. |
| **Tier 5 (Critical Risk)**| Severe ratio deterioration or insolvency risk. | **Decline / Ineligible**. Outside standard risk tolerance thresholds. |

---

## 3. Working Capital & MPBF Assessment (Regulatory Model)

The platform evaluates the **Maximum Permissible Bank Finance (MPBF)** according to established regulatory banking norms (Tandon Committee Method II & Turnover Methodologies):

- **Working Capital Gap (WCG):** Evaluated from total current assets less non-bank current liabilities.
- **Stipulated Net Working Capital (NWC):** Mandatory borrower margin requirement calculated against current asset base.
- **Assessed Bank Finance:** Deterministic calculation ensuring bank exposure complies strictly with regulatory caps and drawing power limits.

---

## 4. Intelligent Schedule Completeness & Fallback Engine

Audited financial reports frequently arrive with missing schedule annexures. The engine incorporates a resilient fallback framework:

1. **Automated Completeness Detection:** Identifies which audited schedules (Debtor Aging, Inventory, Fixed Assets) are attached.
2. **Deterministic Mathematical Fallbacks:** Uses aggregate balance sheet line items to maintain appraisal continuity without stalling underwriters.
3. **Contextual Policy Flags:** Generates highlight flags in the final Credit Appraisal Memo (CAM) requesting document submission prior to final loan disbursement.
