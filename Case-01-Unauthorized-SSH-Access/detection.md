
## Detection Summary

The suspicious activity was detected by the Wazuh security monitoring platform. The Wazuh agent installed on the Ubuntu server collected authentication logs and forwarded them to the manager for analysis.

An alert was generated after multiple failed SSH login attempts were observed within a short time window, indicating possible brute-force behavior.



### Alert Evidence

Figure 1 shows the Wazuh alert generated for repeated SSH authentication failures.

![Wazuh Alert](https://github.com/korw1-ook/SOC-Investigation-Portfolio/blob/main/screenshots/fail_ssh.png?raw=true)


