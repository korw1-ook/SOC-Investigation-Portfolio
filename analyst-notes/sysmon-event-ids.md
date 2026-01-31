# Sysmon – Quick Analyst Notes

Sysmon provides detailed endpoint activity after a system is accessed.

Windows Security logs show **who logged in**.  
Sysmon shows **what happened after login**.

---

## Important Sysmon Event IDs

- **1** – Process creation  
  Shows executed commands and parent process.

- **3** – Network connection  
  Detects outbound connections and possible C2 traffic.

- **10** – Process access  
  LSASS access may indicate credential dumping.

- **11** – File creation  
  Used to detect dropped malware or tools.

- **12 / 13** – Registry creation or modification  
  Common persistence technique.

- **22** – DNS query  
  Useful for identifying suspicious domains.

---

## Common Malicious Patterns

- PowerShell or cmd execution → suspicious  
- Unknown process making network connection → possible C2  
- File drop followed by execution → malware activity  
- Registry run key added → persistence  

---

## Analyst Note

Sysmon events are noisy.  
Single events are not enough — correlation and behavior patterns matter.
