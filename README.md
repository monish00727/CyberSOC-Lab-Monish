# CyberSOC-Lab-Monish
Hands-on SOC Lab using AWS, Splunk, Windows Server, and Linux to simulate enterprise log collection, monitoring, and detection.

# 🧩 Lab Overview
**Architecture**

- AWS EC2 Windows Server
  * Hosted in Cloud
  * Configured with IIS web server
  * Logging Windows Event Logs, IIS logs

- Local Virtual Machines (via VirtualBox/VMware)
  * Windows 10 VM — with Sysmon and Winlogbeat
  * Kali Linux VM — for simulating attacker behavior

- Splunk SIEM
  * Installed locally
  * Ingesting logs from AWS server and VMs
  * Includes custom dashboards and detection queries
    
# 🛠️ Tools Used
  * AWS EC2 (Free Tier)
  * Splunk Enterprise (Trial)
  * Windows Server 2025
  * Kali Linux
  * Sysmon, Winlogbeat
  * Remote Desktop Protocol (RDP)

# 🔍 Key Skills Demonstrated
  * Deploying cloud infrastructure (EC2, security groups, RDP, web server)
  * Setting up centralized log monitoring using Splunk
  * Writing basic SPL (Search Processing Language) detection queries
  * Creating dashboards for login failures, port scans, and suspicious PowerShell activity
  * Configuring and forwarding logs from multiple sources
  * Basic threat simulation (brute-force, enumeration, suspicious commands)
    
# 📘 How to Reproduce This Lab
  1. Create AWS EC2 instance (Windows Server) in Mumbai region
  2. Enable RDP, HTTP in security groups
  3. Install IIS, enable logging
  4. Create two local VMs (Linux + Windows)
  5. Install Splunk and set up forwarders
  6. Simulate suspicious activities (failed RDP, PowerShell misuse)
  7. Monitor and alert using Splunk queries


