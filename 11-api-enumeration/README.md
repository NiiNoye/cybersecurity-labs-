# Lab 11 — API Enumeration

## Objective

Identify and examine API endpoints exposed by the OWASP Juice Shop application and observe their authentication and response behavior.

## Environment

- OWASP Juice Shop
- Kali Linux
- Burp Suite
- Firefox
- Docker
- Host-Only Network

## Testing Methodology

API requests were identified through Burp Suite HTTP History.

### 1. Quantity API

Tested:

```http
GET /api/Quantitys/
