# 🔍 Threat Hunting Methodologies – Windows Environment


## 🧭 Threat Hunting by Tactic

## 🔎 Discovery

Attackers begin by understanding the environment they have compromised.

### Hunting Focus
- Execution of built-in Windows tools used for user, group, and host enumeration.
- Unusual internal network scanning activity.
- Suspicious or unexpected processes initiating LDAP queries.
- Correlating discovery activity using parent–child process relationships.

---

##  Privilege Escalation

After discovery, attackers attempt to gain elevated privileges.

### Hunting Focus
- SYSTEM-level processes spawned by low-privileged user accounts.
- Potential service permission abuse, such as service binary path modification.
- Parent–child process relationships with user context analysis.

---

## 🔐 Credential Access

Credential access allows attackers to expand their access across systems.

### Hunting Focus
- Known indicators associated with LSASS credential dumping.
- Events related to domain controller replication activity.
- Multiple failed authentication attempts followed by a successful login.
- Unusual process creation linked to potentially compromised user accounts.

---

## 🔄 Lateral Movement

Using valid credentials, attackers move from one system to another.

### Hunting Focus
- Unusual process creation initiated by `WmiPrvSE.exe`.
- Suspicious successful authentication patterns indicating potential Pass-the-Hash (PtH) activity.
- Unexpected process execution following successful remote authentication.
- Correlating lateral movement activity back to the source host to identify initial compromise.

---

## 🧠 Attacker Workflow (High-Level)

The hunting methodologies align with the typical attacker thought process:

1. Understand the environment of the compromised system and escalate privileges where possible.
2. Harvest credentials from available credential stores.
3. Move laterally using valid credentials while blending into normal internal traffic.
4. Establish a new foothold on additional systems and repeat the process to maintain persistence.
---

## ⭐ Notes

- This repository serves as a **quick reference** for Windows-based threat hunting.
- The techniques discussed are applicable to **SOC analysis**, **blue team operations**, and **hands-on labs**.
- Behavioural correlation is critical — individual events alone are rarely sufficient.

---
