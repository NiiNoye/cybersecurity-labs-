# Lab 05 — OWASP Juice Shop

## Objective

Deploy OWASP Juice Shop as an intentionally vulnerable web application and use it as the primary target for authorized web application security testing.

## About OWASP Juice Shop

OWASP Juice Shop is a deliberately insecure web application designed for security training, awareness demonstrations, Capture the Flag (CTF) activities, and security tool testing.

The application contains vulnerabilities covering the OWASP Top 10 and additional real-world security weaknesses.

## Lab Environment

- Host: macOS
- Container Platform: Docker
- Security Workstation: Kali Linux
- Web Application: OWASP Juice Shop
- Application Port: 3000

## Architecture

```text
                 macOS Host
                     |
                  Docker
                     |
              Juice Shop Container
                     |
                TCP Port 3000
                     |
             192.168.56.1:3000
                     |
             Host-Only Network
                     |
               Kali Linux
              192.168.56.2
