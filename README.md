# Penetration-Testing-
Penetration Testing of Basic Pentesting 1 Machine using Nmap and Metasploit.

# 🛡️ Penetration Testing Report: Metasploitable2

This repository contains a sample penetration testing project report focused on the vulnerable **Metasploitable2** machine. The objective of this project is to simulate and document the methodology used by attackers to identify and exploit vulnerabilities in outdated systems, using industry-standard tools and techniques.


## 📌 Project Overview

- **Target Machine**: Metasploitable2 (Vulnerable VM)
- **Attacker Machine**: Kali Linux
- **Test Type**: Black-box simulated penetration test
- **Report Format**: PDF/DOCX (included in this repo)

---

## 🧰 Tools Used

| Tool         | Purpose                          |
|--------------|----------------------------------|
| `nmap`       | Port scanning & service detection |
| `enum4linux` | SMB enumeration                  |
| `nikto`      | Web server vulnerability scan    |
| `Metasploit` | Exploitation & post-exploitation |

---

## 📋 Methodology

### 1. 🔍 Reconnaissance & Scanning

- Identified live hosts and scanned open ports.
- Used `nmap -sV -A` to detect services and versions.

### 2. 🧠 Enumeration

- Enumerated SMB users with `enum4linux`.
- Scanned for web vulnerabilities using `nikto`.

### 3. 💥 Exploitation

- Exploited vulnerable **vsftpd 2.3.4** service using Metasploit.
- Gained shell access with `exploit/unix/ftp/vsftpd_234_backdoor`.

### 4. 🔓 Post-Exploitation

- Verified access using `whoami`, `id`, and `uname -a`.
- Located flag: `flag{root_access_granted}`



## 🧠 Lessons Learned

- Importance of patch management and disabling unused services.
- Practical understanding of enumeration techniques.
- Real-world use of Metasploit for automated exploitation.



## 🛡️ Defense Recommendations

- Regularly update and patch services.
- Disable anonymous and unused services.
- Conduct periodic vulnerability assessments.
- Harden access control and restrict external exposure.

  

## 📚 Disclaimer

This project was conducted in a **controlled lab environment** for **educational purposes only**. Do **not** attempt to use these techniques on systems you do not own or have explicit permission to test.



## 📬 Contact

**Author**: Sakshi Sandeep Kumar 
**Institute**: MGM College of Engineering and Technology  
**Email**: sakshisandeep2000@gmail.com_




