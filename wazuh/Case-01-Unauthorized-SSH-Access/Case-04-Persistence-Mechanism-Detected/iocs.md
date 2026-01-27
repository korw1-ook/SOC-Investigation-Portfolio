## Indicators of Compromise (IOCs)


| Type               | Indicator                                           |
| ------------------ | --------------------------------------------------- |
| Created Artifact   | `/etc/systemd/system/update.service`                |
| Persistence Method | systemd service (MITRE T1543.002)                   |
| Affected Host      | Ubuntu Server (Wazuh Agent)                         |
| Log Sources        | `/var/ossec/logs/syscheck.log`, `/var/log/auth.log` |
