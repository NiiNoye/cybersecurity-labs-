# Lab 08 — SQL Injection

## Objective

Understand and demonstrate SQL Injection against an intentionally vulnerable web application in an isolated cybersecurity laboratory.

The exercise focused on how unsafely handled user input can alter the intended logic of a database query.

## Environment

- Security Workstation: Kali Linux
- Target: OWASP Juice Shop
- Proxy: Burp Suite
- Browser: Firefox
- Network: Isolated Host-Only laboratory network
- Target: Local Juice Shop instance

## What is SQL Injection?

SQL Injection occurs when untrusted user input is incorporated into a dynamically constructed SQL statement in a way that allows the input to alter the intended query.

Conceptually, an unsafe application might construct a query like:

```text
SELECT * FROM Users
WHERE email = '<user_input>'
AND password = '<password>';
