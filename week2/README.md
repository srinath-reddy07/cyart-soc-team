# Week 2 - SOC Alert to Response Simulation

## 📌 Objective
To simulate a real-world cyber attack and demonstrate a complete Security Operations Center (SOC) workflow including detection, triage, response, and documentation.

---

## 🛠️ Tools & Technologies Used
- Kali Linux (Attacker Machine)
- Metasploit Framework (Exploitation Tool)
- Metasploitable2 (Vulnerable Target Machine)
- VMware Workstation (Virtual Environment)
- Netstat (Network Evidence Collection)
- SHA256 (Integrity Verification)

---

## ⚔️ Attack Simulation
A known vulnerability in the VSFTPD service was exploited using the Metasploit module:
```
exploit/unix/ftp/vsftpd_234_backdoor
```

- Attacker IP: 192.168.19.129 (Kali Linux)
- Target IP: 192.168.19.120 (Metasploitable)

The exploit resulted in unauthorized root-level access to the target system.

---

## 🚨 Detection & Alert Details
- Alert ID: 001  
- Description: VSFTPD Exploit Detected  
- Priority: Critical  
- Status: Confirmed Incident  

The activity was identified as suspicious and validated as a true positive based on successful exploitation.

---

## 🧠 MITRE ATT&CK Mapping
- **Technique ID:** T1190  
- **Technique Name:** Exploit Public-Facing Application  

This attack falls under the Initial Access tactic in the MITRE ATT&CK framework.

---

## 🔍 Incident Response Process
The incident was handled following SOC best practices:

1. **Detection** – Identified unauthorized access attempt  
2. **Triage** – Classified as Critical based on impact  
3. **Containment** – Target system isolated  
4. **Eradication** – Malicious access removed  
5. **Recovery** – System stabilized  
6. **Documentation** – Incident recorded and analyzed  

---

## 📊 Evidence Collection
- Tool Used: `netstat`
- Data Collected: Active network connections
- Integrity Verification: SHA256 Hash

---

## 📈 Outcome
- Successful exploitation of vulnerable service  
- Root access achieved on target system  
- Complete SOC workflow demonstrated  
- Incident properly analyzed, documented, and mitigated  

---

## 📂 Files Included
- 📄 SOC Report (Detailed PDF with explanation)
- 📸 Screenshots (Attack, Configuration, Evidence)

---

## 📝 Conclusion
This project demonstrates a complete SOC lifecycle from attack simulation to response. It highlights the importance of vulnerability management, continuous monitoring, and structured incident response in cybersecurity operations.
