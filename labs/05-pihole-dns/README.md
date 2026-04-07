# Network-Wide Ad Blocker & DNS Privacy Solution (Pi-hole)

**Tools:** Raspberry Pi 5, Pi-hole, Docker, Linux CLI, DNS/DHCP  
**Year:** 2025

## What I Built
Deployed Pi-hole as a DNS server on a Raspberry Pi 5 running in Docker, blocking ads and trackers at the network level for every device on the home network without touching individual devices.

## What I Did
Configured a static IP for the Pi, set it as the primary DNS server on the router, and pointed upstream queries to Quad9 for privacy. Managed everything through the Linux CLI — service monitoring, blocklist updates, and log review. Achieved a 30-70% query block rate across all connected devices.

## What I Learned
This was my first real exposure to how DNS actually works in practice. Watching query logs in real time showed me how much background traffic devices generate and how DNS-layer blocking works as a lightweight but effective security control.

## Screenshots
*Coming soon*
