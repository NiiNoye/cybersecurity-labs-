# Lab 06 — Burp Suite Web Application Testing

## Objective

Use Burp Suite as an intercepting proxy to capture, inspect, modify, and replay HTTP requests against an intentionally vulnerable web application in the cybersecurity laboratory.

## Environment

- Host: macOS
- Security Workstation: Kali Linux
- Target: OWASP Juice Shop
- Proxy: Burp Suite
- Browser: Firefox
- Target Address: 192.168.56.1:3000

## What is Burp Suite?

Burp Suite is a web application security testing platform that allows security professionals to inspect and manipulate HTTP and HTTPS traffic between a browser and a web application.

In this laboratory, Burp Suite was used to understand how web applications communicate with clients and how security testers can analyze those communications.

## Laboratory Architecture

```text
                Kali Linux
                    |
                 Firefox
                    |
             Burp Suite Proxy
              127.0.0.1:8080
                    |
              Host-Only Network
                    |
             192.168.56.1:3000
                    |
             OWASP Juice Shop
                    |
                  Docker
                    |
               macOS Host
