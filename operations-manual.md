# Operational Compliance & Logic Framework

**Version:** 2.1  
**Focus:** Risk Management, HR Compliance, and Workflow Optimization

## 1. Human Resources Logic
### The "Fingerprint Mandate" (Risk Control)
* **Policy:** No "Pending" starts. Staff/Volunteers cannot begin work until physical FBI background check clearance is received.
* **Workflow:** 1. Candidate submits fingerprints via CCRE.
    2. Physical letter digitized to **Purple Zone** (SharePoint Restricted).
    3. Account access granted only *after* file verification.

### Volunteer Tiered Access (Role-Based Access Control)
* **Tier 1 (Direct Care):** Full background check required. Read-only access to Incident Forms.
* **Tier 2 (Logistics/IT):** No direct client contact. No background check required if supervised. Zero access to client data systems.

## 2. Residential Supervision Protocols
### The Variance Protocol (IoT Integration)
To reduce staffing costs while maintaining safety, operations utilize a state-approved variance allowing for motion-sensor monitoring during overnight shifts.
* **Trigger:** Motion sensors at exits.
* **Alert:** Pager notification to staff quarters.
* **SLA:** Staff must visually verify resident status within **90 seconds**.
* **Audit Trail:** Automated logs serve as legal proof of "active supervision."

## 3. Incident Management Workflow
**Double Reporting Standard:**
In peer-to-peer incidents, two distinct reports are generated to protect privacy in legal discovery:
1.  **Report A (Aggressor):** Classified as "Threat to Others."
2.  **Report B (Victim):** Classified as "Serious Injury/Harm."
*Rationale: Prevents cross-contamination of legal records.*

## 4. Business Continuity (Disaster Recovery)
**The "Offline" Protocol (Internet/Power Loss > 15 mins):**
1.  **Ops:** Switch Salesforce Mobile App to "Offline Mode" (Cached Data).
2.  **Clinical:** Revert to paper "Red Binder" forms using Client IDs only.
3.  **Recovery:** Manual data entry and physical shredding of paper logs upon power restoration.
