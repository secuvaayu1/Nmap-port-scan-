# Nmap-port-scan-
Nmap Network Reconnaissance Report This project contains an Nmap scan report for the local network range 172.26.176.0/20. The scan was performed using both TCP SYN scan and full-port scan to identify active hosts and their open ports.

📋 Steps Followed
Installed Nmap from the official website.

Determined local IP range: 172.26.176.0/20.

Ran TCP SYN scan:

sudo nmap -sS 172.26.176.0/20

Performed full-port scan:
sudo nmap -p- -sS 172.26.176.0/20

Identified hosts and open ports.

Documented results in HTML report.

Provided recommendations for potential security improvements.

Findings
Host 1: 172.26.176.1 (Microsoft Hyper-V/Windows system)

Open TCP ports: 5754, 6850, 7680, 9012, 9013, 53540-53545

Host 2: 172.26.183.233 (Kali Linux)

No open TCP ports detected.

🚨 Potential Risks
Unknown custom services on high ports may expose management/debug interfaces.

Port 7680 linked to Windows Delivery Optimization could be misused for P2P file distribution.

Multiple filtered ports suggest firewall presence, but exposed services still increase attack surface


Summary:-

I scanned my local network 172.26.176.0/20 and found 2 active hosts.
My Kali machine has no open TCP ports, but the other host (172.26.176.1) has multiple open ports, including 5754, 6850, 7680, 9012, 9013, and 53540–53545.
Some ports are unknown/custom, and 7680 is linked to Windows Delivery Optimization.
These could pose risks if misconfigured or unprotected.








