# Cybersecurity Labs

A hands-on cybersecurity learning and practical lab portfolio documenting my journey in cybersecurity.

## About

This repository contains practical security labs, experiments, methodologies, and notes developed while building my cybersecurity skills.

The labs cover areas including:

- Network security
- Web application security
- API security
- Authentication and authorization
- Vulnerability assessment
- Security testing
- Security automation
- Linux
- Python
- Docker
- Burp Suite
- OWASP security concepts

## Lab Environment

### Host

- MacBook Pro 2019
- Intel Core i5
- 8 GB RAM
- macOS

### Virtualization

- VirtualBox
- Kali Linux

### Lab Network

The lab uses an isolated Host-Only network for security testing.

```text
                 Internet
                    |
                 macOS
                    |
              NAT / Internet
                    |
              Kali Linux VM
              /           \
          eth0             eth1
      10.0.2.15       192.168.56.2
                           |
                    Host-Only Network
                           |
                    192.168.56.1
                           |
                    Docker Services
                           |
                    OWASP Juice Shop

