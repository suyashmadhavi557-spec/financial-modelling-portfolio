# Financial Modelling Portfolio

Practice-based financial modelling projects built from real company annual reports, focused on Indian listed companies. Each project is built from scratch in Excel and documented here as I learn.

---

## Project 1: Nestlé India — 3-Statement Model

**File:** Nestle_India_3_Statement_Model.xlsx

### Overview
A fully linked 3-statement financial model (Income Statement, Balance Sheet, Cash Flow Statement) built from Nestlé India's standalone financial statements, covering FY 2023-24 to FY 2025-26.

### Why Nestlé India
Chosen as a first modelling project for its single-segment FMCG business, minimal debt complexity, and clean, consistent reporting — ideal for learning core 3-statement linkages without the noise of multi-segment consolidation or complex financing structures.

### Structure
| Sheet | Contents |
|---|---|
| Income Statement | Revenue, expenses, exceptional items, PBT, tax, PAT — 3 years |
| Balance Sheet | Equity, liabilities, assets — 3 years, with a balance check row |
| Cash Flow Statement | Operating, Investing, Financing activities — 2 years (derived from year-on-year Balance Sheet movement, so requires an opening + closing year) |

### Key Modelling Decisions
- **Standalone financials used** (not consolidated) to keep the model focused on Nestlé India's core entity.
- **Cash Flow Statement copied from the reported financials** rather than fully derived from Balance Sheet movements. Actuarial adjustments embedded in employee benefit provisions and contingency provisions made a from-scratch derivation unreliable without additional actuarial disclosures — so the reported CF was used as the source of truth, with Income Statement lines (PBT, Depreciation, Exceptional Items) still linked live into it.
- **Balance Sheet Cash is linked to the Cash Flow Statement's** ending cash balance rather than hardcoded, so the two statements are structurally connected.
- **Balance check row** (Total Assets − Total Equity & Liabilities) confirms the model balances to zero across all 3 years.

### Checks Performed
- ✅ Balance Sheet balances (Assets = Equity + Liabilities) for all 3 years
- ✅ Cash Flow Statement ties out: Net Increase in Cash matches Ending Cash − Beginning Cash
- ✅ Income Statement figures flow correctly into Cash Flow (PBT, D&A, Exceptional Items)

### What I Learned
- How Ind AS financial statements are structured (Income Statement, Balance Sheet, Cash Flow) and where each disclosure sits in an annual report
- The mechanics of linking statements together so they respond to each other rather than sitting as static figures
- Why real-world items like actuarial provisions and Other Comprehensive Income complicate a textbook cash-flow derivation, and how to make a reasoned modelling trade-off when that happens
- How to build a balance check to validate a 3-statement model is truly linked, not just individually correct

### Source Data
Nestlé India Ltd. Annual Reports (FY 2023-24, FY 2024-25, FY 2025-26), publicly available at:
- [Nestlé India Investor Relations](https://www.nestle.in/investors)
- [BSE India](https://www.bseindia.com/) / [NSE India](https://www.nseindia.com/)

*(Annual report PDFs are not included in this repository — only the derived model. Figures are used solely for educational/portfolio purposes.)*

---

## Roadmap
- **Project 2:** Forecasting — revenue and cost drivers, working capital assumptions, equity roll-forward, and a debt schedule
- **Project 3:** DCF valuation
- **Project 4:** Sensitivity analysis and comparable company analysis

---

## About Me
Built by Suyash Madhavi as part of a self-directed financial modelling skills upgrade, alongside an MMS Finance postgraduate program. Background in accounting (Tally Prime, GST compliance, financial reporting) and mutual fund/portfolio analysis.
