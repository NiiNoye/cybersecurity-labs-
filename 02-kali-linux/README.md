# Lab 02 — Kali Linux Security Environment

## Objective

Set up and configure Kali Linux as the primary penetration testing and cybersecurity analysis environment for the home laboratory.

## Environment

- Host OS: macOS
- Virtualization: VirtualBox
- Guest OS: Kali Linux
- Network Mode: NAT + Host-Only

## Kali Linux Role

Kali Linux serves as the security workstation for the laboratory.

It provides access to a wide range of tools for:

- Network reconnaissance
- Vulnerability assessment
- Web application security testing
- Password security testing
- Digital forensics
- Traffic analysis
- Exploitation in authorized environments
- Security research

## Network Configuration

Kali Linux was configured with two network interfaces.

### Interface 1 — NAT

```text
Interface: eth0
Address: 10.0.2.15/24
Purpose: Internet connectivity
