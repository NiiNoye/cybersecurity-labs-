# Lab 9 — Broken Access Control

## Objective

Test whether authenticated users can access resources or functionality that should be restricted to other users or roles.

## Environment

- OWASP Juice Shop
- Kali Linux
- Burp Suite
- Firefox
- Docker
- Host-Only Network

## Testing Performed

### 1. Administrative Access

Attempted to access the Juice Shop administration interface while authenticated as a normal student user.

Result:

```text
403 Forbidden
