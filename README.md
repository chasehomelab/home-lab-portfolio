Home Lab Portfolio
Chase Marshall | Cybersecurity Student | U.S. Air Force Veteran
LACC Cybersecurity A.S. (GPA 3.7) | CompTIA Security+ Candidate | Targeting SOC Analyst / IT Support Roles

Projects
1. Active Directory Lab
Tools: Windows Server 2022, Active Directory Domain Services, Group Policy, PowerShell, DNS, DHCP
Overview:
Deployed and configured Active Directory Domain Services on Windows Server 2022. Built a new forest (lab.local), managed user accounts and OUs via GUI and PowerShell, enforced Group Policy password and lockout policies, configured DNS records and DHCP scopes, mapped network drives via command line, and performed remote desktop support sessions.
Key Skills Demonstrated:

Active Directory installation and domain configuration
Full user lifecycle management — provisioning, password resets, offboarding
Group Policy hardening (password complexity: 12 chars, account lockout: 5 attempts)
PowerShell AD automation — New-ADUser, Set-ADAccountPassword, Search-ADAccount
DNS A record creation and nslookup verification
DHCP scope configuration and static reservations
Network drive mapping via net use command
Windows Event Viewer security log analysis (Event ID 4624/4625)
Remote Desktop Protocol (RDP) support simulation

What I Learned:
How enterprise environments manage users, permissions, and security policies at scale — the core of what help desk and sysadmin roles deal with daily.

2. SIEM Monitoring Lab (Splunk Enterprise) — Multi-Source
Tools: Splunk Enterprise, Windows Server 2022, Kali Linux, Metasploitable 2, SPL
Overview:
Deployed Splunk Enterprise on Windows Server 2022 and configured it to ingest logs from 4 sources: Windows Security, Application, and System event logs, plus Linux syslog from Metasploitable 2. Built a multi-source SOC monitoring dashboard with panels for log volume, failed login detection, Linux host activity, and top security events. Created automated alerts for brute force and web enumeration attacks.
Key Skills Demonstrated:

SIEM deployment and multi-source log ingestion
Windows Event Log and Linux syslog forwarding (UDP 514)
SPL query writing — stats, timechart, where, search
Automated alert creation (brute force: 3+ failed logins, web enumeration: 3+ 404s)
Multi-panel SOC dashboard creation
Cross-platform event correlation

What I Learned:
How real SOC teams monitor multiple log sources simultaneously and how SIEM tools correlate events across platforms to surface threats automatically.

3. Vulnerability Scanning Lab (OpenVAS/Greenbone)
Tools: Greenbone Vulnerability Manager (GVM/OpenVAS), Kali Linux, Metasploitable 2, VirtualBox
Overview:
Deployed Greenbone Vulnerability Manager on Kali Linux and ran a Full and Fast vulnerability scan against Metasploitable 2 in an isolated virtual network. Analyzed 62 findings by CVSS severity and cross-referenced all critical CVEs with successful Metasploit exploits.
Key Findings:

14 Critical | 9 High | 39 Medium | 4 Low (Max CVSS: 10.0)
Critical CVEs: vsftpd 2.3.4, Samba usermap_script, distcc daemon, UnrealIRCd backdoor

Key Skills Demonstrated:

Vulnerability scanner deployment and configuration
Full and Fast scan execution against live target
CVE identification and CVSS severity triage
Correlating scanner findings with manual exploitation results
Report generation and documentation

What I Learned:
How vulnerability scanners surface attack surface the way a real SOC or pen test team would — and how scanner findings map directly to exploitable CVEs.

4. End-to-End Attack & Detection Lab (Capstone)
Tools: Kali Linux, Metasploit Framework, Metasploitable 2, OpenVAS, Splunk Enterprise, Apache, Wireshark, Windows Server 2022, VirtualBox
Overview:
Built a three-VM lab simulating a complete enterprise attack and SOC detection scenario. Exploited four critical vulnerabilities identified by OpenVAS, detected attacks in Splunk SIEM in real time, deployed a web server and forwarded access logs to the SIEM, created web attack detection alerts, and analyzed all traffic using Wireshark.
Lab Architecture:

Attacker: Kali Linux (192.168.56.105)
Victim: Metasploitable 2 (192.168.56.103)
Defender/SOC: Windows Server 2022 + Splunk (192.168.56.104)

Attack Chain:

Ran OpenVAS Full and Fast scan — identified 4 critical CVEs
Exploited vsftpd 2.3.4 backdoor → root shell (uid=0)
Exploited Samba usermap_script → root shell
Exploited distcc daemon → daemon shell
Exploited UnrealIRCd backdoor → root shell
Configured syslog forwarding from Metasploitable 2 to Splunk
Deployed Apache web server on Kali; forwarded access logs to Splunk
Created SPL alert for web enumeration (multiple 404s from single host)
Analyzed all attack traffic in Wireshark — TCP flags, port scan signatures, backdoor connections on port 6200

Key Skills Demonstrated:

Multi-vector exploitation using Metasploit Framework
SIEM log ingestion and real-time attack detection
Apache web server deployment and log management
SPL-based web attack detection rule writing
Wireshark packet analysis — ICMP, HTTP, TCP handshake, SYN scan identification
Full attack lifecycle: reconnaissance → exploitation → detection → documentation

What I Learned:
How a SOC analyst sees an attack in progress — and how understanding the attacker's perspective makes you a better defender. This lab demonstrates both offensive and defensive security skills in a single end-to-end exercise.

5. Network-Wide Ad Blocker & DNS Privacy Solution (Pi-hole)
Tools: Raspberry Pi 5, Pi-hole, Linux CLI, DNS/DHCP
Overview:
Deployed Pi-hole DNS server on a Raspberry Pi 5, blocking ads and trackers at the network level for all connected devices. Achieved a 30-70% query block rate. Handled static IP reservation, upstream DNS configuration using Quad9, and service management via Linux CLI.
Key Skills Demonstrated:

Linux server deployment and configuration
DNS and DHCP fundamentals
Network-level security hardening
Raspberry Pi administration
Service monitoring and management


6. WireGuard VPN Server
Tools: Raspberry Pi 5, WireGuard, Linux CLI, UFW Firewall
Overview:
Self-hosted a WireGuard VPN server on a Raspberry Pi 5 to encrypt home network traffic and practice secure remote access. Managed key generation, peer configuration, and firewall rules in a Linux environment.
Key Skills Demonstrated:

VPN server deployment and configuration
Public/private key cryptography concepts
Linux firewall rule management
Secure remote access implementation
Network traffic encryption


Tools & Technologies
CategoryToolsSIEMSplunk Enterprise, SPLVulnerability ScanningGreenbone/OpenVAS, NmapExploitationMetasploit FrameworkPacket AnalysisWiresharkIdentity & AccessActive Directory, Group Policy, PowerShellWeb ServerApacheTicketingJiraOSKali Linux, Windows Server 2022, Ubuntu, Metasploitable 2VirtualizationVirtualBoxScriptingBash, PowerShellHome Lab InfraRaspberry Pi 5 (Pi-hole, WireGuard)

Certifications & Training

TryHackMe Pre Security Certificate
TryHackMe SEC0 path — passed
TryHackMe Cyber Security 101 — in progress (68%)
CompTIA Security+ (SY0-701) — exam scheduled Summer 2026
LACC Cybersecurity A.S. — GPA 3.7- expecteded graduation spring 2027
