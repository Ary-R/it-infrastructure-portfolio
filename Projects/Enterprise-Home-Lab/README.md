
## Project Status

🚧 In Progress

Current Phase:
- ✅ Architecture Design
- 🔄 VMware Environment Setup
- ⏳ pfSense Deployment
- ⏳ Ubuntu Server Configuration
- ⏳ Cloudflare Tunnel Integration
- ⏳ Security Testing
- ⏳ Documentation

# Enterprise Cybersecurity Home Lab

A virtualized enterprise cybersecurity home lab designed to simulate a secure corporate network environment using VMware. This project demonstrates network segmentation, firewall configuration, secure web hosting, and authorized security testing through a realistic enterprise architecture.

---

# Project Overview

This home lab replicates a small enterprise network by implementing industry-standard security practices. The environment is built using virtual machines running on VMware and consists of multiple isolated network zones managed by pfSense Firewall.

The lab focuses on:

- Enterprise network segmentation
- Firewall policy implementation
- Secure web server deployment
- Cloudflare Tunnel integration
- Authorized penetration testing
- Traffic monitoring and future security monitoring integration

---

# Objectives

- Design a secure enterprise network architecture
- Implement network segmentation using LAN, DMZ, and Security Testing zones
- Configure pfSense as the central firewall and routing gateway
- Deploy an Ubuntu Nginx Web Server securely through Cloudflare Tunnel
- Perform authorized penetration testing using Kali Linux
- Develop hands-on experience with enterprise cybersecurity technologies

---

# Technologies Used

| Category | Technology |
|----------|------------|
| Virtualization | VMware Workstation |
| Firewall | pfSense |
| Operating System | Ubuntu Server |
| Security Testing | Kali Linux |
| Web Server | Nginx |
| Secure Access | Cloudflare Tunnel |
| Monitoring (Future) | Wazuh / Syslog |
| Network Analysis | Wireshark |
| Vulnerability Assessment | Nmap, Nikto, Burp Suite |

---

# High-Level Architecture

The high-level architecture provides an overview of the enterprise network and illustrates how external users securely access the web server through Cloudflare Tunnel while pfSense protects and segments the internal network.

<img width="950" height="230" alt="High-Level Architecture" src="https://github.com/user-attachments/assets/995ab4e5-a1fd-49b3-bb67-714fce34a23f" />

### Architecture Summary

- Internet traffic enters through Cloudflare Tunnel.
- Cloudflare securely forwards traffic to the Ubuntu Nginx Web Server.
- pfSense acts as the central firewall and router.
- The enterprise network is divided into three isolated security zones:
  - LAN
  - DMZ
  - Security Testing

---

# Detailed Architecture

The detailed architecture illustrates the complete virtual infrastructure, including virtualization, network segmentation, firewall rules, virtual machines, and authorized security testing paths.

<img width="1500" height="1500" alt="Detailed Architecture" src="https://github.com/user-attachments/assets/e7406c45-2e90-4a26-b1fe-273cdbf18fcb" />


### Network Zones

## LAN Zone (192.168.10.0/24)

Purpose:

- Internal administration
- Secure SSH management
- System configuration

Device:

- Ubuntu Admin Workstation

---

## DMZ Zone (192.168.20.0/24)

Purpose:

Host public-facing services while remaining isolated from the internal network.

Services:

- Ubuntu Server
- Nginx Web Server
- HTTPS
- Cloudflare Tunnel Agent

---

## Security Testing Zone (192.168.30.0/24)

Purpose:

Provide a dedicated environment for authorized penetration testing and vulnerability assessment.

Device:

- Kali Linux VM

Security Tools:

- Nmap
- Wireshark
- Burp Suite
- Nikto

---

# Firewall Design

pfSense serves as the central security gateway for all virtual networks.

Firewall Policies:

✅ Internet → DMZ (HTTPS)

✅ LAN → DMZ (SSH)

✅ Security Testing → DMZ

❌ Internet → LAN

❌ DMZ → LAN

❌ Security Testing → LAN

These rules ensure that public-facing services remain isolated while allowing controlled administrative and security testing access.

---

# Traffic Flow

Normal User Access

Internet

↓

Cloudflare Tunnel

↓

pfSense Firewall

↓

Ubuntu Nginx Web Server

---

Authorized Security Assessment

Kali Linux

↓

pfSense Firewall

↓

Ubuntu Nginx Web Server

Only authorized penetration testing traffic is permitted from the Security Testing Zone.

---

# Project Features

- Enterprise Network Segmentation
- Virtualized Infrastructure
- pfSense Firewall
- Secure DMZ Design
- Cloudflare Tunnel Integration
- Ubuntu Nginx Web Server
- SSH Administration
- Penetration Testing Environment
- Firewall Policy Enforcement
- Future Security Monitoring Integration

---

# Future Enhancements

Planned improvements include:

- Wazuh Security Monitoring
- Centralized Syslog Server
- Intrusion Detection System (IDS)
- Intrusion Prevention System (IPS)
- VPN Remote Access
- SIEM Dashboard
- Docker Services
- Network Traffic Analytics

---

# Repository Structure

```text
Enterprise-Home-Lab/
│
├── README.md
├── diagrams/
├── docs/
├── configs/
├── screenshots/
└── scripts/
```

---

# Skills Demonstrated

- Network Architecture Design
- Network Segmentation
- Firewall Configuration
- Linux Administration
- Web Server Deployment
- Cloud Security
- Penetration Testing
- Network Security
- System Hardening
- Enterprise Documentation

---

# Disclaimer

<img width="450" height="250" alt="Ary_Disclaimer" src="https://github.com/user-attachments/assets/a633b88b-e347-44f1-a537-1aa9e28b0f90" />

