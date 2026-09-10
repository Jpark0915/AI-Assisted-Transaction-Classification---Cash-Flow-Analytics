# AI-Assisted-Transaction-Classification---Cash-Flow-Analytics

## Project Overview

This project demonstrates an end-to-end financial analytics workflow using Excel, Power Query, and Generative AI to transform raw banking and credit-card transaction data into a structured dataset and interactive dashboard.

The workflow combines transaction data from a Bank of America checking account and a Discover credit card, classifies transactions using rule-based logic, routes ambiguous expenses to AI-assisted review, and uses human verification to evaluate the AI classifications.

The goal was to build a practical analytics workflow that emphasizes **data quality, classification accuracy, human validation, and business insights** rather than simply creating visualizations.

---

## Business Problem

Raw financial transaction exports often contain inconsistent descriptions, different transaction types, transfers, credit-card payments, refunds, and ambiguous merchant names.

Before meaningful spending analysis can be performed, the data needs to be:

- Combined from multiple sources
- Standardized
- Classified into meaningful transaction types
- Separated into true spending versus non-spending activity
- Categorized by merchant and spending category
- Validated for accuracy

This project addresses these challenges through a rule-first classification workflow supported by Generative AI and human review.

---

## Key Questions

The analysis was designed to answer questions such as:

- How much was spent during the analysis period?
- Which spending categories accounted for the most spending?
- Which merchants received the most spending?
- How did spending change month-to-month?
- How much recorded income was received?
- How accurately could AI classify previously unresolved expenses?
- How can automated classification reduce manual data-cleaning work?

---

## Tools Used

- **Microsoft Excel** — Data analysis, formulas, dashboard, and reporting
- **Power Query** — Data ingestion, transformation, standardization, and rule-based transaction classification
- **Generative AI** — Classification of unresolved expense descriptions
- **Human Validation** — Verification of AI-generated categories
- **GitHub** — Documentation and portfolio presentation

---

## Project Workflow

The project followed a rule-first classification approach:

```text
Raw Bank & Credit Card Data
            ↓
      Data Standardization
            ↓
   Transaction Type Rules
            ↓
     Manual Review Queue
            ↓
      Approved Transaction Types
            ↓
      Merchant Rule Matching
            ↓
   ┌─────────────────────────┐
   │ Expense already matched │
   │         by rules        │
   └────────────┬────────────┘
                │
                ↓
        Category Assigned

Unresolved Expenses
            ↓
     AI-Assisted Review
            ↓
      Human Verification
            ↓
     Final Category
            ↓
      Spending Analysis
            ↓
       Excel Dashboard
