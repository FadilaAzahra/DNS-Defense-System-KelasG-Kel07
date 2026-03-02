IP Address Planning
Network Configuration

Network Type: Host-Only Adapter
Subnet: 192.168.30.0/24
Subnet Mask: 255.255.255.0
Gateway: 192.168.30.1
Environment: Isolated Cybersecurity Lab

IP Address Table

Hostname: Kali Linux (Attacker)
IP Address: 192.168.30.100
OS: Kali Linux
Role: Attacker

Hostname: Ubuntu + DVWA (Target)
IP Address: 192.168.30.5
OS: Ubuntu Server
Role: Web Server (Victim)

Hostname: Security Onion (Monitoring)
IP Address: 192.168.30.200
OS: Security Onion
Role: IDS / SIEM

System Details

Attacker Machine
IP Address: 192.168.30.100
Tools: Nmap, Hydra
Target IP: 192.168.30.5

Target Server
IP Address: 192.168.30.5
Services: Apache Web Server, MySQL, SSH
Open Ports: 80 (HTTP), 443 (HTTPS), 22 (SSH)

Monitoring Server
IP Address: 192.168.30.200
Management Ports: 22 (SSH), 443 (HTTPS)
Monitoring Mode: Passive Network Capture
Function: Network Traffic Analysis and Intrusion Detection
