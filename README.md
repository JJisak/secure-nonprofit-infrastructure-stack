# Turnkey Secure Non-Profit Infrastructure Stack (PoC)

## Project Overview
This project represents a Proof of Concept (PoC) for a "Zero Cost," high-compliance technical infrastructure designed for residential non-profit organizations operating in high-liability environments (e.g., trafficking survivor care). 

The goal was to engineer a system that balances **absolute data privacy** (HIPAA/VAWA compliance) with **operational transparency** for donors, utilizing a stack of integrated, free-tier enterprise tools.

## Business Objectives
* **Cost Efficiency:** Designed a full ERP/CRM stack utilizing $0/year non-profit licenses (Salesforce Power of Us, Microsoft 365 Nonprofit, Carepatron).
* **Risk Mitigation:** Created a "Traffic Light" data policy to segregate sensitive clinical data (Red Zone) from public operational data (Green Zone).
* **Scalability:** Architecture supports global operations (US, East Africa) with low-bandwidth synchronization protocols.

## Technical Stack & Architecture
This project integrates the following systems into a unified ecosystem:

* **CRM & Database:** Salesforce NPSP (Non-Profit Success Pack)
* **Electronic Health Records (EHR):** Carepatron (HIPAA Compliant)
* **Identity & Access Management:** Microsoft 365 (Entra ID) / Role-Based Access Control (RBAC)
* **Data Collection:** Microsoft Forms & Power Automate (Logic Flows)
* **Payment Processing:** Zeffy (API integration for 0% fee processing)

## Key Deliverables
1.  **[Master Technology & Data Map](technology-data-map.md):** A blueprint of API integrations, data flow, and security protocols.
2.  **[Operational Compliance Framework](operations-manual.md):** Standard Operating Procedures (SOPs) mapping technical tools to legal requirements (Virginia Code, HIPAA, VAWA).

## Highlights for Recruiters/Hiring Managers
* **Data Governance:** Defined rigid protocols for PII (Personally Identifiable Information) handling across international borders.
* **Automation:** Concepted "One-Way" data valves allowing volunteers to submit incident reports without accessing sensitive client databases.
* **Disaster Recovery:** Designed "Offline Protocols" for internet/power loss scenarios to ensure business continuity.
