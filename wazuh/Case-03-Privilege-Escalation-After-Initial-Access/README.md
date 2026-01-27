# Case – Privileged Command Execution After SSH Login

This case documents the investigation of privileged command execution
observed after a successful SSH login to an Ubuntu Linux server.

Following initial access, additional security alerts were generated
indicating the use of elevated privileges. The activity required
analysis to determine whether privilege escalation was attempted.

---

## Case Objective

To investigate whether commands executed after SSH login indicate:

- legitimate administrative activity, or
- potential privilege escalation following initial access.

---

## File Reading Order

1. **scenario.md**  
   Describes the post-login activity and investigation scope.

2. **timeline.md**  
   Shows the sequence of authentication and command execution events.

3. **investigation.md**  
   Documents analysis of logs related to privileged command usage.

4. **detection.md**  
   Explains how privileged command execution was detected.

5. **iocs.md**  
   Lists relevant indicators observed during the investigation.

6. **mitre.md**  
   Maps the activity to MITRE ATT&CK techniques.

7. **conclusion.md**  
   Summarizes findings and determination.

---

## Environment

- Ubuntu Linux Server  
- Wazuh monitoring agent  
- SSH service enabled  

---

## Notes

This case focuses on post-authentication behavior and is intended to
evaluate detection and investigation of privilege-related activity
after initial access.
