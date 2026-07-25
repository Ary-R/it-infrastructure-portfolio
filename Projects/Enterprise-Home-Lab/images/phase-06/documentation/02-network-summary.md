# Network Configuration Summary

## Enterprise Network

The home lab is segmented into multiple security zones using pfSense Firewall.

---

## LAN Zone

**Subnet**

192.168.10.0/24

Purpose

* Internal administration
* Secure management
* SSH access

---

## DMZ Zone

**Subnet**

192.168.20.0/24

Purpose

* Public-facing web services
* Isolated server environment

---

## Security Testing Zone

**Subnet**

192.168.30.0/24

Purpose

* Authorized penetration testing
* Vulnerability assessment

---

## Virtual Machines

| System        | Role              |
| ------------- | ----------------- |
| pfSense       | Firewall & Router |
| Ubuntu Server | Apache Web Server |
| Kali Linux    | Security Testing  |

---

## Network Security

All traffic between network zones is controlled through pfSense Firewall to ensure proper segmentation and restricted communication.
