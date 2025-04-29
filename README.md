# OSCP Machine Lab Environment

This document describes a customized penetration testing lab designed to simulate real-world OSCP scenarios. Participants are expected to enumerate, exploit, escalate privileges, and document their findings.

---

## 🖥️ Target: Windows 1
- **OS Version:** Windows 10
- **Objective:** Initial Access and Privilege Escalation
- **Target IP:** Must be discovered during enumeration
- **Download:** [Windows 1 Image](https://drive.google.com/file/d/12vErA_VWcPTrUxufWvmeVwFqj8By2s-p/view?usp=sharing)

---

## 🐉 Target: Ubuntu 2
- **OS Version:** Ubuntu Server
- **Objective:** Initial Access and Privilege Escalation
- **Target IP:** `10.4.4.10`
- **Download:** [Ubuntu 2 Image](https://drive.google.com/file/d/17olsIcVQ_pgD917KmVWOZTRKpSAQBgFt/view?usp=sharing)

---

## 🖥️ Target: Windows 3
- **OS Version:** Windows 7 Professional
- **Objective:** Initial Access
- **Target IP:** `10.5.5.20`
- **Download:** [Windows 3 Image](https://drive.google.com/file/d/10Dj0wL5K05sG_kSAlLmnm0iH9Pcy6yjS/view?usp=sharing)

---

## 🏢 Target: Active Directory Domain Controller
- **OS Version:** Windows Server 2022
- **Objective:** Initial Access and Domain Enumeration
- **Target IP:** `10.5.5.1`
- **Download:** [AD DC Image](https://drive.google.com/file/d/147FPYesLQuJuyWX13tme9UneITzaoRNC/view?usp=sharing)

> ⚡ **Note:** If access is gained, you can connect via **RDP** (Remote Desktop Protocol).

---

## 🛠️ Assessment Methodology
- Conduct comprehensive enumeration.
- Exploit misconfigurations or known vulnerabilities.
- Perform post-exploitation enumeration.
- Develop your own privilege escalation paths.
- Document each step for reporting purposes.

---

## 🧩 Recommended Approach
- Start with full port scans and service enumeration.
- Gather as much information as possible before exploitation.
- Analyze findings carefully — avoid rushing exploits.
- Keep detailed notes on each step taken.

---

## ⚙️ Lab Usage Guidelines

If your computer resources are limited and you cannot run all machines simultaneously, follow this workflow:

1. **Start with Windows 1**  
   Perform initial access and privilege escalation on Windows 1.
2. **Use Windows 1 (if needed) to attack Ubuntu 2**  
   Complete initial access and privilege escalation on Ubuntu 2.
3. **After finishing with Ubuntu 2, shut it down**  
   Free up resources for the next targets.
4. **Ensure the Active Directory Domain Controller is powered on**  
   The AD DC must always be running throughout the engagement.
5. **Attack Windows 3**  
   - Initially keep Windows 3 powered off.
   - After successfully enumerating domain users, power on Windows 3 and capture the required flags.

> **Important:** The **Active Directory Domain Controller must always stay powered on**.

---

## 📋 Notes
- No predefined exploit paths are provided.
- Participants are responsible for their own research and exploitation.
- Adopt a real-world mentality: assume limited information is available.
- Practical reporting is expected, including both successful and failed attempts.

---

## 📚 Resources
- [HackTricks](https://book.hacktricks.xyz/)
- [PayloadsAllTheThings](https://github.com/swisskyrepo/PayloadsAllTheThings)
- [GTFOBins](https://gtfobins.github.io/)
- [OSCP Preparation Guide](https://www.offsec.com/)
- [Active Directory Attack Mindmap](https://hausec.com/2019/10/23/active-directory-attack-map/)

---

## ⚠️ Disclaimer
This environment is for educational purposes only. Unauthorized use of these techniques outside controlled environments is illegal.
