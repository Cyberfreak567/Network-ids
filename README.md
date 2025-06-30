# Network-ids
# Suricata on Parrot Os
**Suricata** is a powerful, open-source, high-performance **Network Threat Detection Engine** developed by the Open Information Security Foundation (OISF). It provides capabilities such as:

- Deep packet inspection
- Signature-based intrusion detection (IDS)
- Network intrusion prevention (IPS)
- Protocol detection & TLS inspection
- Real-time alerting and logging
Installed Version - 6.0.10

This project showcases a basic Network Intrusion Detection System (NIDS) using Suricata to:
Detect ICMP Echo Requests (ping scans)
Detect HTTP GET requests (web activity)

# **Video**

https://github.com/user-attachments/assets/fee5da08-9c16-471d-8090-18d01d043fb8

# 🛠️ Installation Steps
sudo apt update
sudo apt install suricata -y

Enable HTTP Parsing
sudo nano /etc/suricata/suricata.yaml

# 🚦 Running Suricata
sudo suricata -c /etc/suricata/suricata.yaml -i ens33

# Testing 
ICMP: ping google.com
Http: curl http://testphp.vulnweb.com/

# Check Alerts
sudo tail -f /var/log/suricata/fast.log
