# SOC Investigation Portfolio

This repository contains a collection of SOC-style incident investigation case studies created in a simulated security monitoring environment using Wazuh and Linux system logs.

Each case study represents a realistic security incident scenario and demonstrates the complete investigation process followed by a Security Operations Center (SOC) analyst — from alert detection to final remediation recommendations.

The purpose of this portfolio is to showcase practical SOC skills including alert analysis, log investigation, timeline reconstruction, IOC identification, MITRE ATT&CK mapping, and incident documentation.

---

## Investigation Environment

- Operating Systems: Ubuntu Linux (monitored endpoint)
- Monitoring Platform: Wazuh
- Data Sources:
  - Linux authentication logs
  - System logs
  - File Integrity Monitoring (FIM)
- Analysis Method: Evidence-based incident investigation

---

## Case Studies Overview

### Case 01 — Unauthorized SSH Access Attempt
**Category:** Initial Access

**Summary:**  
Investigation of multiple SSH authentication failures originating from an external IP address. The activity was analyzed to determine whether unauthorized access had occurred.

**Key Skills Demonstrated:**
- Alert triage and validation
- Authentication log analysis
- Identification of brute-force behavior
- IOC extraction
- MITRE ATT&CK mapping

---

### Case 02 — Successful Login After Brute Force
**Category:** Account Compromise

**Summary:**  
Analysis of repeated SSH authentication failures followed by a successful login from the same source IP, indicating potential credential compromise.

**Key Skills Demonstrated:**
- Event correlation
- Detection of successful brute-force activity
- Timeline reconstruction
- Identification of compromised accounts
- Incident severity assessment

---

### Case 03 — Privilege Escalation After Initial Access
**Category:** Post-Compromise Activity

**Summary:**  
Investigation of privileged command execution following a successful remote login. The activity was analyzed to determine whether privilege escalation was attempted.

**Key Skills Demonstrated:**
- Post-access behavior analysis
- Sudo activity investigation
- Correlation between login and privilege usage
- Detection of elevation attempts
- Security control evaluation

---

### Case 04 — Persistence Mechanism Detected on Linux Host
**Category:** Persistence

**Summary:**  
Investigation of system modifications including unauthorized user creation and scheduled task changes, indicating attempts to maintain long-term access.

**Key Skills Demonstrated:**
- Persistence technique identification
- File Integrity Monitoring (FIM) analysis
- User and cron modification detection
- Long-term threat assessment
- Remediation planning

---

## Investigation Methodology

Each case study follows a structured SOC investigation workflow:

1. Alert detection and validation  
2. Log review and evidence collection  
3. Timeline reconstruction  
4. Indicator of Compromise (IOC) identification  
5. MITRE ATT&CK technique mapping  
6. Impact assessment  
7. Remediation and monitoring recommendations  

This approach reflects real-world SOC operations and incident response practices.

---

## Skills Demonstrated

- SOC alert triage
- Linux log analysis
- Wazuh rule interpretation
- Incident investigation methodology
- Attack lifecycle understanding
- MITRE ATT&CK framework usage
- Technical documentation and reporting

---

## Disclaimer

All incidents documented in this repository were generated in a controlled lab environment for educational and demonstration purposes only.  
No production systems were affected.

---





