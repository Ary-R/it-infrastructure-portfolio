# Security Assessment Summary

## Assessment Scope

The Ubuntu Apache Web Server was assessed from the Kali Linux Security Testing Zone.

---

## Tools Used

* Nmap
* Curl
* WhatWeb
* Gobuster
* Nikto
* Wireshark

---

## Security Improvements

Implemented:

* Apache version disclosure reduction
* Security response headers
* Apache module hardening
* SSH hardening
* Service validation

---

## Verification

Security improvements were verified through:

* Manual HTTP header inspection
* Apache service validation
* Directory enumeration
* Web server fingerprinting
* Vulnerability scanning

---

## Conclusion

The implemented hardening measures reduced unnecessary information disclosure and improved the overall security posture of the Apache web server while maintaining normal functionality.
