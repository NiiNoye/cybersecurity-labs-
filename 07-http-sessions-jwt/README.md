# Lab 07 — HTTP Sessions, Authentication & JWT Security

## Objective

Analyze authentication traffic and JSON Web Tokens (JWTs) in an intentionally vulnerable web application to understand how authentication and session-related security mechanisms work.

## Environment

- Security Workstation: Kali Linux
- Target: OWASP Juice Shop
- Proxy: Burp Suite
- Browser: Firefox
- Network: Isolated Host-Only laboratory network
- Authentication mechanism: JWT

## Authentication vs Authorization

### Authentication

Authentication determines:

> Who is the user?

Examples include:

- Username/password verification
- Session authentication
- Token-based authentication

### Authorization

Authorization determines:

> What is the authenticated user allowed to do?

Authentication and authorization are separate security controls.

## Capturing the Login Request

Burp Suite HTTP History was used to inspect the Juice Shop login process.

The login request was observed as an HTTP POST request.

A typical request structure included:

```http
POST /rest/user/login
Content-Type: application/json
