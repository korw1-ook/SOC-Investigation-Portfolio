# Hunting suspicious activities indicating initial user or host compromise(ssh).

Starting with this scenario, we will use the filebeat-* index and hunt for brute-forcing attempts via SSH on our jumphost server on July 3, 2023. 

To start hunting, I will use the Visualize Library  and create a visualisation table using Lens

## Evidence

KQL:  host.name: jumphost AND event.category: authentication AND system.auth.ssh.event: Failed

![SSH Bruteforce](images/ssh.png)


---
Now we can observed the count of failed login attempted of apecific user.hese two IP addresses and accounts are highly notable since they generated over 500 failed authentication events within the given timeframe.

Now we will find the sucessfull authentication.

## Evidence

KQL: host.name: jumphost AND event.category: authentication AND system.auth.ssh.event: Accepted AND source.ip: (167.71.198.43 OR 218.92.0.115) 

![SSH Bruteforce](images/authentication.png)

## conclusion

we have confirmed that the attacker from 167.71.198.43 accessed the Jumphost server using the dev account.