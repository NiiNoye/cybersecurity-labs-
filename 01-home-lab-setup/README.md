# Lab 01 — Home Cybersecurity Lab Setup

## Objective

Build an isolated cybersecurity laboratory environment for practicing penetration testing, vulnerability assessment, web application security, network security, and security tooling.

## Environment

### Host Machine

- MacBook Pro 2019
- Intel Core i5
- 8 GB RAM
- macOS

### Virtualization

- VirtualBox
- Kali Linux

### Containerization

- Docker

### Security Applications

- Burp Suite
- OWASP Juice Shop
- Nmap
- cURL
- Firefox

## Lab Architecture

```text
                    Internet
                       |
                    macOS Host
                       |
                ----------------
                |              |
              NAT          Host-Only
                |              |
             Kali VM      192.168.56.0/24
                |              |
          10.0.2.15       192.168.56.1
                               |
                         Docker Services
                               |
                        OWASP Juice Shop
