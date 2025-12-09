FCCS End-to-End Hands-On Portfolio (Oracle EPM Cloud)

This repository is my complete Financial Consolidation & Close Cloud Service (FCCS) hands-on implementation project, designed to demonstrate real-world skills equivalent to 2.5+ years practical experience.

The purpose of this repo is to simulate a production-like FCCS environment with:

Metadata modeling

Data loading (manual + automated)

Consolidation and elimination

Journals

Intercompany

Automated data pipelines using EPM Automate

Smart View analysis

Process documentation

End-to-end project structure for interviews

Integration with EPBCS + EDMCS in later stages

This project will grow step-by-step as I complete hands-on tasks.

📌 1. Project Objectives

Build a fully functional FCCS application from scratch

Demonstrate hands-on knowledge for job interviews

Build a strong GitHub portfolio showcasing real work

Create reusable assets: metadata templates, data files, scripts

Practice every minor FCCS topic in detail

📁 2. Folder Structure
fccs-portfolio/
│
├── README.md                 ← Project documentation
├── LICENSE                   ← MIT license
│
├── metadata/                 ← Account, Entity & other dimension files
│   ├── Entity.csv
│   └── Account.csv
│
├── data/                     ← Actuals / journals / intercompany data
│   └── Actuals_Q1_2025.csv
│
├── automations/              ← Scripts for EPM Automate (coming soon)
│   └── (placeholders added)
│
└── docs/                     ← Screenshots, results, process docs
    └── (placeholders added)

📌 3. Metadata Included (Phase 1)
✔ Entity Hierarchy

Simple parent–child structure:

Level	Entity	Parent
0	Global	—
1	HeadOffice	Global
1	OpCo1	Global
1	OpCo2	Global
✔ Account Hierarchy

Basic P&L + Balance Sheet accounts:

Total Revenue → Revenue

Total Expense → Expense

Total Assets → Cash, Receivables

📌 4. Data Included (Phase 1)
Actuals_Q1_2025.csv

Contains sample monthly Actuals for Jan 2025 (P&L + Cash):

Entity	Account	Period	Value
HeadOffice	Revenue	2025-01	150000
OpCo1	Revenue	2025-01	50000
OpCo2	Revenue	2025-01	40000
…	…	…	…

This dataset is used for:

Data Load

Validation

First consolidation run

📌 5. How to Use This Repository
✔ Prerequisites

To run this project end-to-end, you need:

Oracle FCCS subscription / access

EPM Automate installed

Smart View installed

Basic understanding of Oracle EPM Cloud navigation

📌 6. Steps Covered in Phase 1
Step 1 — Project Setup

Create GitHub repo

Add metadata & data files

Document structure (this README)

Step 2 — Metadata Load

Using FCCS UI:

Navigator → Overview → Dimensions → Import Metadata


Or via EPM Automate:

epmautomate uploadFile Entity.csv
epmautomate importMetadata "Entity.csv" Entity

epmautomate uploadFile Account.csv
epmautomate importMetadata "Account.csv" Account

Step 3 — Data Load

Using Data Load Rules or EPM Automate.

Step 4 — Run Consolidation

Using FCCS Console or EPM Automate:

epmautomate runBusinessRule "FCCS_Consolidation"

📌 7. Future Enhancements (Coming Soon)
✔ Phase 2 — Data Load & Journal Entries
✔ Phase 3 — Intercompany & Eliminations
✔ Phase 4 — Cash Flow Automation
✔ Phase 5 — EPM Automate Pipeline
✔ Phase 6 — Reporting & Smart View Templates
✔ Phase 7 — EPBCS + EDMCS Integration
📌 8. Purpose of This Repository

This repository serves as evidence of my hands-on FCCS experience and demonstrates:

Application setup skills

Metadata expertise

Consolidation understanding

Data management and automation

Real-time troubleshooting

📌 9. Contact

For any queries related to this project or FCCS implementation experience:

Name: Devaharsha
Email: (Optional: add if you want recruiters to contact you)
LinkedIn: (Optional)

End of README
