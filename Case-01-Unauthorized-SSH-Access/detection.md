
## Detection Summary

The suspicious activity was detected by the Wazuh security monitoring platform. The Wazuh agent installed on the Ubuntu server collected authentication logs and forwarded them to the manager for analysis.

An alert was generated after multiple failed SSH login attempts were observed within a short time window, indicating possible brute-force behavior.



![Wazuh Alert](screenshots/wazuh-alert.png)
