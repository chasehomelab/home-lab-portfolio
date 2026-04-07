# SIEM Monitoring Lab (Splunk Enterprise)

**Tools:** Splunk Enterprise, Windows Server 2022, Kali Linux, Metasploitable 2, SPL  
**Year:** 2025

## What I Built
Deployed Splunk Enterprise on Windows Server 2022 and configured it to ingest logs from four sources simultaneously — Windows Security, Application, and System event logs, plus Linux syslog from Metasploitable 2. Built a multi-panel SOC monitoring dashboard and wrote automated detection alerts.

## What I Did
Set up log forwarding from both Windows and Linux hosts, wrote SPL queries to surface failed logins, track log volume by source, and monitor Linux host activity. Created an automated brute force alert triggering on 3+ failed logins from a single host, then simulated an actual attack to validate the detection end-to-end. Also built a web enumeration alert for multiple 404s from a single IP.

## What I Learned
This lab made SIEM work feel real. Writing a detection rule is one thing — watching it fire on traffic you generated yourself is different. It also showed me how much context you lose when you're only monitoring one log source.

## Screenshots
*Coming soon*
