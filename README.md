FCCS Hands-On Portfolio – End-to-End Implementation

This repository contains my complete Financial Consolidation & Close Cloud Service (FCCS) hands-on work, built step-by-step to demonstrate practical experience equivalent to 2.5+ years of implementation and support.

The goal of this project is to simulate a real-world FCCS environment including:

Application setup

Metadata design & loading

Actuals data preparation & load

Consolidation

Reporting

Automation using EPM Automate

End-to-end documentation

This repository also integrates with EPBCS and EDMCS in later phases.

📌 Phase 1 — Environment & Metadata Setup

This phase includes:

Application provisioning

Tools setup (Smart View, EPM Automate)

Metadata design for Accounts & Entities

Minimal working hierarchy for consolidation testing

Files included:
File	Description
metadata/Entity.csv	Basic parent-child Entity hierarchy
metadata/Account.csv	Accounts for P&L + Balance Sheet
data/Actuals_Q1_2025.csv	Sample actuals for one period to run consolidation
📌 Phase 2 — Data Load & Consolidation

Steps covered:

1. Prepare Metadata & Data Files

Entity hierarchy

Account hierarchy

Actuals file for Jan 2025

2. Upload using FCCS UI or EPM Automate

Example commands (documented in later phases):

epmautomate uploadFile Entity.csv
epmautomate importMetadata Entity.csv "Entity"
epmautomate uploadFile Actuals_Q1_2025.csv
epmautomate importData Actuals_Q1_2025.csv "DataLoadRule"

3. Run Consolidation

Navigate to Consolidation → Run Full Consolidation

Or via EPM Automate:

epmautomate runBusinessRule "FCCS_Consolidation_Full"

4. Validate in Smart View

Connect to the FCCS instance

Retrieve consolidated balances at Global entity level

📌 Phase 3 — Automation (Coming Soon)

Backup automation scripts

Data load automations

Consolidation cycles

Email notifications

📌 Phase 4 — Reporting (Coming Soon)

Smart View reports

Narrative Reporting package

Financial Statements

📌 Folder Structure
fccs-portfolio/fccs/
├─ README.md
├─ metadata/
│  ├─ Entity.csv
│  └─ Account.csv
├─ data/
│  └─ Actuals_Q1_2025.csv
├─ automations/
│  └─ (scripts coming next)
└─ docs/
   └─ (documentation coming next)

🚀 About This Project

This portfolio is part of my end-to-end learning plan to master FCCS from 0 → Expert level with real hands-on implementation.
Every step is validated manually and documented for interview preparation.

If you are a recruiter or hiring manager, this repository shows:

Strong understanding of the FCCS data model

Practical consolidation experience

Experience with automation tools

Familiarity with reporting & workflow# fccs-portfolio
