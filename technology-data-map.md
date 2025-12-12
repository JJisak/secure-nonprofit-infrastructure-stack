# Master Technology & Data Map v2.6

**Scope:** Domestic (Virginia) & International (Egypt, Kenya, Zambia)  
**Core Philosophy:** "Traffic Light" Data Segregation

## 1. The "Traffic Light" Security Framework
To ensure compliance with HIPAA (Medical Privacy) and VAWA (Safety), data is segregated into three zones based on sensitivity.

| Status | Zone Name | System | Security Level | Authorized Users | Data Policy |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 🔴 | **Red Zone (Clinical)** | Carepatron (EHR) | Strict HIPAA | Clinical Directors, Nurses, Licensed Staff | **Real Names Allowed.** Encrypted. Strictly NO volunteer access. |
| 🟣 | **Purple Zone (Ops)** | Microsoft 365 | High (BAA Signed) | Admin Staff, Shift Supervisors | **Client IDs Only** (e.g., CLT-004). No real names in file names. |
| 🟢 | **Green Zone (Public)** | Salesforce NPSP | Standard | Fundraising, Board, Volunteers | **Anonymized Metrics.** Donors see "100 bed nights," never "Jane Doe." |

## 2. Integrated Tech Stack
### Core Infrastructure
* **Network Security:** OpenDNS Family Shield configured at the router level to block high-risk content categories.
* **Hardware:** Standardization on enterprise-grade refurbished units (Dell Latitude/Lenovo ThinkPad) to reduce CapEx by ~65%.
* **Compliance:** Microsoft 365 HIPAA Business Associate Agreement (BAA) active.

### Data Flow & Automation
**Problem:** Volunteers need to report incidents but cannot see clinical history.
**Solution (The "Volunteer Valve"):**
1.  **Input:** Volunteer submits Microsoft Form ("Shift Report") using Client ID.
2.  **Logic:** Power Automate flow analyzes input.
    * *If "Aggression":* Triggers High Priority email to Director.
    * *If "Routine":* Archives data to SharePoint List.
3.  **Result:** One-way data flow (Up to clinicians, never down to volunteers).

## 3. Global Architecture (Salesforce)
**Egypt Scholarship Program (Experience Cloud)**
* **Public Access:** Guest User Screen Flows allow students to apply without licenses.
* **Data Objects:** Custom "Service Delivery" objects track tuition payments and asset tracking (Laptop Serial Numbers).

**Field Communications (Low Bandwidth)**
* **Routine:** WhatsApp (E2E Encrypted).
* **High Sensitivity:** Signal with "Sealed Sender" enabled to minimize metadata risks in politically sensitive regions.
