# Lab 10 — BOLA / IDOR

## Objective

Demonstrate Broken Object Level Authorization (BOLA), also commonly known as Insecure Direct Object Reference (IDOR), by testing whether one authenticated user can access another user's resource by modifying an object identifier.

## Environment

- OWASP Juice Shop
- Kali Linux
- Burp Suite
- Firefox
- Docker
- Host-Only Network

## Test Accounts

Two separate local test accounts were used:

- Student A
- Student B

No real user accounts or credentials were used.

## Testing Methodology

Student B was authenticated and accessed their own basket:

```http
GET /rest/basket/7
