## Investigation Findings

Log analysis confirmed that a user-level account successfully authenticated to the system via SSH. Shortly after the login event, multiple sudo commands were executed.

The close timing between the login and privileged command execution, combined with the external origin of the session, indicates an attempt to elevate privileges beyond the initially obtained access.

Such behavior is uncommon for normal user activity and is consistent with post-compromise privilege escalation attempts.



### Log Evidence

![Sudo Activity](screenshots/sudo-log.png)
