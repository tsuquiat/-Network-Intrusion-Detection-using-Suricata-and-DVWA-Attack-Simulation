# -Network-Intrusion-Detection-using-Suricata-and-DVWA-Attack-Simulation
This project deploys Suricata as an IDS in a controlled lab. It simulates real-world attacks against DVWA to analyze Suricata’s traffic inspection. The environment includes Kali Linux, a vulnerable DVWA server, and a monitoring system for alert generation.

# Technologies Used:
- Suricata (IDS )
- Kali Linux (attacker machine)
- Ubuntu Server (target system)
- DVWA – Damn Vulnerable Web Application
- Nmap
- SQLMap
# Attack Scenarios:
1️. SQL Injection Attack
- Automated SQL injection using sqlmap
- Extraction of database information from DVWA
- Detection through Suricata alert rules

2️. Network Reconnaissance
- Nmap scans (SYN scan, service detection, OS fingerprinting)
- Detection of scanning behavior by Suricata rules

3️. Cross-Site Scripting (XSS)
- Injection of malicious scripts into DVWA
- Detection using custom Suricata HTTP rules
# Suricata and DVWA Configuration:
configure DVWA:
https://github.com/digininja/DVWA

use this documentation to install and configure suricata: https://docs.suricata.io/en/latest/quickstart.html 

Main steps:
1. Install Suricata
sudo apt install suricata suricata-update
2. Update rules
sudo suricata-update
3. Configure network interface in:
 /etc/suricata/suricata.yaml
4. Start Suricata
sudo suricata -i [interface]
# Objectives:
✔ Deploy Suricata IDS in a simulated network  
✔ Detect real cyber attack scenarios  
✔ Analyze Suricata alert logs  
✔ Create custom detection rules  


