# OAuth 2.0

## What is OAuth 2.0?

OAuth 2.0 is an authorization framework that allows one application to access another application's resources on behalf of a user without sharing the user's password.

---

## Why is OAuth Important?

OAuth improves security by allowing applications to use access tokens instead of passwords.

Examples include:

- Sign in with Google
- Sign in with Microsoft
- Sign in with GitHub

---

## Key Components

### Resource Owner

The user.

### Client

The application requesting access.

### Authorization Server

Verifies the user's identity and issues an access token.

### Resource Server

The API that provides the requested data.

---

## Access Token

A temporary credential used to access protected resources.

Example:

Authorization: Bearer eyJhbGciOi...

---

## Refresh Token

Used to obtain a new access token after the current one expires.

---

## Common OAuth Errors

### Invalid Token

Cause:
The access token is expired or invalid.

Solution:
Generate a new access token.

---

### Missing Authorization Header

Cause:
The API request does not include the Authorization header.

Solution:
Include:

Authorization: Bearer <access_token>

User
   │
   ▼
Application
   │
   ▼
Authorization Server
   │
   ▼
Access Token
   │
   ▼
Resource Server(API)
---

## Summary

OAuth 2.0 provides secure authorization by allowing applications to access resources without exposing user passwords.