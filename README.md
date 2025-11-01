# CRSP and Compustat Merging Project

This project demonstrates the process of **merging CRSP (Center for Research in Security Prices)** and **Compustat Fundamentals** datasets using both **Stata** and **SAS**.  
It highlights best practices in financial data integration and variable matching for firm-level analysis.

---

##  Objectives

1. Extract firm-level data from both CRSP and Compustat.
2. Clean and standardize key identifiers (e.g., PERMNO, GVKEY, CUSIP).
3. Merge datasets to align market and accounting variables.
4. Validate the merge by checking match rates, duplicates, and unmatched records.
5. Compare and verify results across Stata and SAS implementations.

---

##  Methodology Overview

###  Data Preparation
- Standardize identifiers (GVKEY, PERMNO, and CUSIP).  
- Apply date alignment rules for fiscal vs. market data.  
- Remove duplicate observations or missing identifiers.

###  Merge Execution
- Conduct one-to-one or many-to-one merges depending on the dataset granularity.  
- Retain firm characteristics and market data in a combined panel.  

###  Post-Merge Validation
- Summarize match statistics.
- Output counts of matched, unmatched, and duplicate rows.
- Export a final merged dataset for further analysis.

---

##  Outputs

- **Merged dataset:** Firm-level panel combining CRSP and Compustat variables.  
- **Merge summary log:** Counts of successful matches and non-matches.  
- **Descriptive report:** Short PDF explaining any discrepancies between Stata and SAS merges.

---

##  Tools & Environment

| Tool | Purpose |
|------|----------|
| **Stata** | Data merging and validation (Firm A) |
| **SAS** | Parallel merge and verification (Firm B) |
| **CRSP / Compustat** | Primary financial data sources |
| **Excel / CSV** | For summary table exports |
