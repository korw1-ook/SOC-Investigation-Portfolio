## Detection Summary

The Wazuh monitoring platform detected the execution of privileged commands through analysis of Linux authentication logs.

Alerts were generated for sudo command usage shortly after a remote login session was established, indicating potential privilege escalation activity.



### Alert Evidence

![Wazuh Alert](screenshots/wazuh-privilege-alert.png)
