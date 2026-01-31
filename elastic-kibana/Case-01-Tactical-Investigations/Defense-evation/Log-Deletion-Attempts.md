# Hunting of Log Deletion Attempts

we will still use the winlogbeat-* index and hunt for log deletion attempts from employee workstations on July 3, 2023. 


## Evidence

The simplest way to detect the deletion of Windows Event Logs is via Event ID 1102.

These events are always generated when a user attempts to delete Windows Logs, so we will use this in our KQL query to hunt for this activity.

**KQL** : host.name: WKSTN-* AND winlog.event_id: 1102

![image](../images/defense-evation/log.png)

## conclusion
Based on the results, it can be seen that Windows Event Logs were cleared from WKSTN-1