# pfSense Interface Configuration

## Overview

pfSense CE acts as the core firewall and router for the Enterprise Home Lab environment.

It provides:

- Network routing
- Firewall enforcement
- Network segmentation
- NAT connectivity

---

## Interface Assignment

| Interface | Purpose | Network |
|---|---|---|
| WAN | External connectivity through VMware NAT | DHCP |
| LAN | Internal infrastructure network | 192.168.10.0/24 |
| OPT1 | Security testing network | 192.168.30.0/24 |

---

## Network Segmentation

### LAN Network

Purpose:
- Internal infrastructure communication
- Ubuntu Server hosting environment

### Security Testing Network

Purpose:
- Controlled penetration testing
- Kali Linux security activities

Network separation allows security testing to be performed without affecting the internal infrastructure environment.
