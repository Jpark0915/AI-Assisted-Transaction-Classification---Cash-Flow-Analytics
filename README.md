# Transaction Classification & Cash Flow Analytics

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#transaction-classification--cash-flow-analytics)

## Project Overview

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#project-overview)

This project uses multi-source transaction data as a case study to demonstrate how messy financial data can be transformed into a structured dataset for analysis. The workflow combines Excel, Power Query, rule-based classification, Generative AI, and human verification to classify transactions and identify spending patterns.

The goal of the project is not just to summarize spending, but to demonstrate a repeatable data analytics workflow that improves data quality, handles ambiguous transactions, and turns raw transaction records into actionable insights.

> **Privacy Note:** The original analysis uses private financial transaction data that is not included in this repository. All public datasets are synthetic and contain no personal banking information.

## Business Problem

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#business-problem)

Transaction exports from different financial accounts often use inconsistent descriptions, formats, and transaction types. Before the data can be analyzed, transactions must be standardized and classified into meaningful categories.

Manual classification can also become time-consuming when transaction descriptions are unclear or inconsistent.

This creates a data quality problem: analysts need a process that can standardize transactions, apply consistent classification rules, handle ambiguous records, and verify results before using the data for reporting.

## Key Questions

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#key-questions)

- How can transaction data from multiple financial accounts be standardized into one dataset?
- Which transactions can be reliably classified using rule-based logic?
- How can Generative AI assist with ambiguous transaction descriptions?
- How accurate are AI-assisted classifications after human verification?
- Which spending categories and merchants represent the largest portions of total spending?
- How can the final data be communicated through an interactive Excel dashboard?

## Tools Used

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#tools-used)

- Excel: data analysis, formulas, validation, and dashboard development
- Power Query: data cleaning, transformation, standardization, and rule-based classification
- Generative AI: classification suggestions for unresolved transaction descriptions
- GitHub: project documentation, version control, and reproducibility

## Project Workflow

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#project-workflow)

1. Imported transaction data from multiple financial accounts into Excel.
2. Standardized transaction fields and formats using Power Query.
3. Applied rule-based logic to classify transaction types such as expenses, transfers, payments, refunds, and income.
4. Isolated unresolved expense transactions that could not be confidently classified using existing rules.
5. Used Generative AI to suggest merchant and category classifications for unresolved transactions.
6. Human-verified AI suggestions and measured classification accuracy.
7. Combined the verified results into a final analysis-ready dataset.
8. Built an interactive Excel dashboard to analyze spending by category, merchant, and month.

## Key Insights

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#key-insights)

### 1. Dining was the largest spending category

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#1-dining-was-the-largest-spending-category)

Dining represented 41.94% of total spending, making it the largest spending category in the dataset.

### 2. Shopping represented the second-largest spending category

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#2-shopping-represented-the-second-largest-spending-category)

Shopping represented 31.66% of total spending, making it the second-largest category after Dining.

### 3. Amazon was the largest individual merchant

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#3-amazon-was-the-largest-individual-merchant)

Amazon represented the largest individual merchant by spending, with $889.59 in classified spending.

### 4. Spending peaked in June 2025

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#4-spending-peaked-in-june-2025)

Monthly spending reached its highest point at $388.99 in June 2025. The lowest monthly spending occurred in April 2026 at $41.99.

### 5. AI-assisted classification achieved 97% accuracy

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#5-ai-assisted-classification-achieved-97-accuracy)

The workflow routed 33 unresolved expense transactions to Generative AI for suggested classifications. After human verification and category normalization, 32 of the 33 AI-assisted classifications were correct, resulting in a 97.0% classification accuracy rate.

This demonstrates how AI can support data classification while human validation remains important for ambiguous cases.

## Dashboard

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#dashboard)

![Transaction Analytics Dashboard](screenshots/dashboard.png)

The dashboard summarizes spending across categories, merchants, and monthly trends while providing high-level spending and income KPIs.

### Key Metrics

- **Transactions Processed:** 268
- **Total Spending Analyzed:** $4,166.94
- **AI-Assisted Reviews:** 33
- **AI Classification Accuracy:** 97.0%
- **Final Transactions Needing Review:** 0

## AI-Assisted Classification

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#ai-assisted-classification)

The classification workflow was designed to use rules first and Generative AI only when existing rules could not confidently classify a transaction.

AI-generated classifications were not automatically accepted. Each suggestion was reviewed and verified before being incorporated into the final dataset.

![AI Classification Review](screenshots/ai_review.png)

This approach helped balance automation with data quality by using deterministic rules for straightforward transactions while reserving AI assistance for more ambiguous cases.

## Final Takeaway

[svg](https://github.com/Jpark0915/ai-assisted-transaction-classification-cash-flow-analytics#final-takeaway)

This project demonstrates how a structured analytics workflow can transform messy, multi-source transaction data into a reliable dataset for business analysis.

By combining Power Query transformations, rule-based classification, Generative AI, human verification, and Excel dashboarding, the project shows how analysts can use automation and AI to improve data preparation without treating AI outputs as automatically correct.

The final workflow provides a practical example of using data quality, validation, and visualization to turn raw transaction records into meaningful financial insights.
