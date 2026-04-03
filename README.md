# Home Lab Portfolio
### Chase Marshall | Cybersecurity Student | U.S. Air Force Veteran

---

## Projects

### 1. SIEM Monitoring Lab (Splunk Enterprise)
**Tools:** Splunk Enterprise, Windows Server 2022, SPL

**Overview:**
Deployed Splunk Enterprise SIEM on Windows Server 2022 and configured it to ingest Windows Security event logs. Built a dashboard to visualize failed login attempts and wrote an automated alert to detect brute force attacks when an account exceeds 3 failed logins within a short window.

**Key Skills Demonstrated:**
- SIEM deployment and configuration
- Windows event log ingestion and parsing
- SPL (Search Processing Language) query writing
- Automated threat detection and alerting
- Security dashboard creation

**What I Learned:**
How real SOC teams monitor for brute force attacks and how SIEM tools correlate log data to surface threats automatically.

---
### 2. Active Directory Home Lab
**Tools:** Windows Server 2022, Active Directory Domain Services, Group Policy, PowerShell

**Overview:**
Deployed and configured Active Directory Domain Services on Windows Server 2022. Built a new forest (lab.local), created and managed user accounts and Organizational Units via both GUI and PowerShell, applied Group Policy password enforcement, created security groups, and configured shared network folders with permission-based access control.

**Key Skills Demonstrated:**
- Active Directory installation and domain configuration
- User account and OU management
- Group Policy Object (GPO) creation and enforcement
- PowerShell bulk user creation and account management
- NTFS and share permissions with security groups

**What I Learned:**
How enterprise environments manage users, permissions, and security policies at scale — the core of what help desk and sysadmin roles deal with daily.

---
### 3. Penetration Testing Lab (Kali Linux + Metasploitable 2)
**Tools:** Kali Linux, Metasploit Framework, Nmap, Wireshark, VirtualBox

**Overview:**
Built a virtualized attack lab using Kali Linux and Metasploitable 2. Performed full reconnaissance workflow including port scanning, service enumeration, and OS fingerprinting with Nmap. Exploited a known CVE backdoor vulnerability (vsftpd 2.3.4) using Metasploit Framework to achieve a root shell, then extracted password hashes from /etc/shadow for offline cracking. Captured and analyzed network traffic using Wireshark identifying DNS, HTTP, and QUIC protocols.

**Key Skills Demonstrated:**
- Network reconnaissance and service enumeration
- Vulnerability identification and exploitation
- Metasploit Framework operation
- Packet capture and protocol analysis
- Post-exploitation techniques

**What I Learned:**
The full offensive security workflow from recon to exploitation — and how understanding attacks makes you a better defender.

---
### 4. Network-Wide Ad Blocker & DNS Privacy Solution (Pi-hole)
**Tools:** Raspberry Pi 5, Pi-hole, Linux CLI, DNS/DHCP

**Overview:**
Deployed and configured Pi-hole DNS server on a Raspberry Pi 5, blocking ads and trackers at the network level for all connected devices. Achieved a 30-70% query block rate across 5-15 active clients. Handled static IP reservation, upstream DNS configuration using Quad9, Wi-Fi interface troubleshooting, and service management via Linux CLI.

**Key Skills Demonstrated:**
- Linux server deployment and configuration
- DNS and DHCP fundamentals
- Network-level security hardening
- Raspberry Pi administration
- Service monitoring and management

**What I Learned:**
How DNS works at a practical level and how network-wide filtering can be implemented as a security control on any network.

---
### 5. WireGuard VPN Server
**Tools:** Raspberry Pi 5, WireGuard, Linux CLI, UFW Firewall

**Overview:**
Self-hosted a WireGuard VPN server on a Raspberry Pi 5 to encrypt home network traffic and practice secure remote access. Managed key generation, peer configuration, and firewall rules in a Linux environment.

**Key Skills Demonstrated:**
- VPN server deployment and configuration
- Public/private key cryptography concepts
- Linux firewall rule management
- Secure remote access implementation
- Network traffic encryption

**What I Learned:**
How VPNs work at a technical level including key exchange, tunneling, and how to secure remote connections — directly relevant to enterprise remote access solutions.

---
6. Vulnerability Scanning Lab (OpenVAS/Greenbone)
Tools: Greenbone Vulnerability Manager (OpenVAS), Kali Linux, Metasploitable 2, VirtualBox
Overview:
Deployed Greenbone Vulnerability Manager (GVM) on Kali Linux and configured it to perform a full vulnerability scan against a Metasploitable 2 target in an isolated virtual network. Analyzed scan results by severity, identified critical CVEs, and cross-referenced findings with exploits previously executed manually using Metasploit Framework.
Key Skills Demonstrated:

Vulnerability scanner deployment and configuration
Network target setup and host-only adapter configuration
Full and Fast scan execution against a live target
CVE identification and CVSS severity triage
Correlating scanner findings with known exploits (vsftpd 2.3.4, Samba, distcc, UnrealIRCd)
Report generation and documentation

What I Learned:
How vulnerability scanners surface attack surface the way a real SOC or pen test team would — and how findings like vsftpd 2.3.4 map directly to exploits I've already executed, completing the full scan → identify → exploit kill chain.
