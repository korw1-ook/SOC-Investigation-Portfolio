# Case 04 – Persistence Mechanism Detected

This case documents the investigation of persistence-related activity
detected on an Ubuntu Linux system following earlier post-authentication
and privileged command execution events.

Security alerts indicated potential attempts to maintain long-term access
to the system, requiring investigation to determine whether a persistence
mechanism was established.

---

## Case Objective

To investigate whether system changes observed after initial access
represent legitimate administrative activity or an attempt to maintain
persistent access.

---

## File Reading Order

1. **scenario.md**  
   Describes the persistence-related activity and investigation scope.

2. **timeline.md**  
   Shows the sequence of events leading to persistence detection.

3. **investigation.md**  
   Documents analysis of system and log evidence.

4. **detection.md**  
   Explains how persistence activity was detected.

5. **iocs.md**  
   Lists indicators identified during investigation.

6. **mitre.md**  
   Maps activity to MITRE ATT&CK persistence techniques.

7. **conclusion.md**  
   Summarizes findings and final determination.

---

## Environment

- Ubuntu Linux Server  
- Wazuh monitoring agent  
- System-level logging enabled  

---

## Notes

This case focuses on identifying persistence mechanisms such as
startup modifications, scheduled tasks, or configuration changes
used to maintain continued access to the system.
