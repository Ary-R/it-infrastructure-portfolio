# Final Apache Configuration

## Objective

Secure the Apache web server by reducing information disclosure and implementing recommended HTTP security configurations.

---

## Configuration Changes

### Server Information Protection

* ServerTokens set to **Prod**
* ServerSignature set to **Off**

These settings reduce unnecessary server information exposed to clients.

---

## HTTP Security Headers

The following response headers were configured:

* X-Content-Type-Options: nosniff
* X-Frame-Options: SAMEORIGIN
* Referrer-Policy: strict-origin-when-cross-origin

These headers improve browser-side security and reduce common web attack vectors.

---

## Apache Modules

Disabled:

* status module

Removing unnecessary modules reduces the server attack surface.

---

## Validation

Configuration changes were verified by:

* Apache configuration testing
* Apache service restart
* Manual HTTP header verification using curl
* Security assessment using Kali Linux

---

## Result

The Apache web server successfully applied the hardening configuration while maintaining normal web service functionality.
