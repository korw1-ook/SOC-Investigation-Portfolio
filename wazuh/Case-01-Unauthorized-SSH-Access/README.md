# Case 1 – SSH Brute Force Detection

This case documents the investigation and detection of SSH brute-force activity
in a controlled lab environment using Wazuh.

All analysis and documentation are separated into individual files for clarity.

---

## Case Files

Read the files in the following order:

1. **scenario.md**  
   Describes the attack scenario and objective.

2. **timeline.md**  
   Shows the sequence of events observed during the attack.

3. **investigation.md**  
   Documents log analysis and investigation steps.

4. **detection.md**  
   Explains how the activity was detected in Wazuh.

5. **iocs.md**  
   Lists indicators observed during the investigation.

6. **mitre.md**  
   Maps the activity to MITRE ATT&CK techniques.

7. **conclusion.md**  
   Summarizes findings and lessons learned.

---

## Goal

To understand how SSH brute-force activity appears in Linux logs and how it can be
detected using correlation-based rules.

---

## Environment

- Kali Linux (attacker)
- Ubuntu Server (target)
- Wazuh (SIEM / detection)

---

## Notes

This case is part of a personal SOC learning lab and focuses on detection and
analysis rather than exploitation.
