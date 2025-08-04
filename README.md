# task1-network-scan
# 🎯 Objective
To scan the local network for open TCP ports using Nmap and analyze potential security risks based on the findings.

# 🛠 Tools Used
 -Nmap v7.95 / v7.97
 -Operating Systems: Windows 10, Kali Linux (VirtualBox)
 -Terminal / Command Prompt
 -Optional: Wireshark (not used in this case)

# 🔄 Steps Performed
  1 Installed Nmap on both Windows and Kali Linux systems.
  2 Identified local IP addresses and subnet range.
  3 Ran TCP SYN scan using nmap -sS <IP-range>.
  4 Saved scan results as text files.
  5 Took screenshots of scanning and setup.
  6 Researched and analyzed open ports for potential vulnerabilities.

# 📊 Scan Results Summary
  Windows:
  
 | Port | State | Service            | Description                                     |
 | ---- | ----- | ------------------ | ----------------------------------------------- |
 | 135  | open  | **msrpc**          | Microsoft RPC – used for Windows services       |
 | 139  | open  | **netbios-ssn**   | NetBIOS Session Service – older Windows sharing |
 | 445  | open  | **microsoft-ds**   | SMB (file sharing) – used in Windows networking |
 | 902  | open  | **iss-realsecure** | Often VMware related (for remote management)    |
 | 912  | open  | **apex-mesh**      | May relate to VMware or other software agents   |

 Linux:
| Port       | State | Service | Description                                     |
| ---------- | ----- | ------- | ----------------------------------------------- |
| **53/tcp** | open  | domain  | DNS server – typically used for name resolution |


# 🖼️ Screenshots
All screenshots are available in the 'Screenshot for Windows' and 'Screenshot for Linux' folder:
-Windows and Linux terminal scans
-Nmap installation confirmation
-IP range detection

# 📁Files Included
  

# ✅ Conclusion
This task helped identify live hosts and exposed ports within the local network. Ports like 445, 135, and 139 pose potential security risks and should be monitored or blocked if unnecessary.
 
