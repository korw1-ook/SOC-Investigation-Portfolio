
## Investigation Findings

Review of authentication logs confirmed multiple failed SSH login attempts followed by a successful authentication for a valid user account.

The failed and successful login events originated from the same external IP address and occurred within a short time interval, indicating credential guessing activity that resulted in account compromise.

Such behavior is inconsistent with legitimate user access and strongly suggests a successful brute-force attack.


### Log Evidence

![Authentication Logs](https://github.com/korw1-ook/SOC-Investigation-Portfolio/blob/main/screenshots/ssh_accepted.png?raw=true)
