
# Windows Security Event IDs – Analyst Reference

This file contains commonly used Windows Security Event IDs that are useful during SOC investigations.

---

## 🔐 Authentication Events

- **4624** – Successful logon  
  Used to identify who logged in, from where, and using which logon type.

- **4625** – Failed logon  
  High volume may indicate brute-force or password spraying.

- **4634** – Logoff  
  Used to track session duration.

- **4672** – Special privileges assigned to new logon  
  Indicates admin-level access (very important).

---

## 👤 Account Management

- **4720** – User account created  
  Possible persistence or unauthorized account creation.

- **4726** – User account deleted  

- **4722** – User account enabled  

- **4725** – User account disabled  

- **4732** – User added to a local security group  
  Critical if added to Administrators group.

- **4733** – User removed from a local group  

- **4740** – User account locked out  
  Often linked with brute-force attempts.

---

## 🧠 Privilege & Policy Changes

- **4670** – Permissions on an object were changed  

- **4719** – System audit policy changed  
  Very suspicious if done unexpectedly.
  

---

## ⚙️ Service & System Activity

- **4697** – Service installed on the system  
  Common persistence technique.

- **7045** – New service installed (System log, very important)
- **1102** – Audit log was cleared
- **5001** – Windows Defender disabled

---

## 🧭 Scheduled Tasks

- **4698** – Scheduled task created  
- **4699** – Scheduled task deleted  
- **4700** – Scheduled task enabled  
- **4701** – Scheduled task disabled  

Often used for persistence.

---

## 🧨 Process & Execution (Limited visibility)

- **4688** – New process created  
  (Only visible if process auditing is enabled)

Useful for basic execution tracking when Sysmon is not available.

---

