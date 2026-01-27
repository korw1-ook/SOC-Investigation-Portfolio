## Investigation Findings

During the investigation, Linux authentication logs were reviewed to validate the alert.

Analysis of the logs revealed multiple failed SSH login attempts targeting different user accounts. All attempts originated from a single external IP address and occurred within a short duration.

This pattern is not consistent with normal administrative behavior and strongly suggests an automated brute-force attempt.


### Log Evidence

Figure 2 shows authentication log entries confirming repeated failed SSH login attempts.

![Authentication Logs](https://github.com/korw1-ook/SOC-Investigation-Portfolio/blob/main/screenshots/fail_ssh-auth.png?raw=true)

