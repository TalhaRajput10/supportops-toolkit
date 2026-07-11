# API Error Troubleshooting Guide

## Purpose

This guide explains common API errors, their possible causes, and the first troubleshooting steps.

---

## 400 Bad Request

Meaning:
The request sent by the client is invalid.

Possible Causes:
- Missing required fields
- Invalid JSON format
- Incorrect parameters

First Checks:
- Verify the request body.
- Check required parameters.
- Validate the JSON syntax.

---

## 401 Unauthorized

Meaning:
Authentication failed.

Possible Causes:
- Invalid API key
- Expired access token
- Missing Authorization header

First Checks:
- Verify the API key.
- Generate a new access token.
- Confirm the Authorization header is included.

---

## 403 Forbidden

Meaning:
The request is authenticated, but the user does not have permission.

Possible Causes:
- Insufficient user permissions
- Incorrect account role
- Restricted resource

First Checks:
- Verify user permissions.
- Check account role.
- Confirm the correct API endpoint is being used.

---

## 404 Not Found

Meaning:
The requested resource could not be found.

Possible Causes:
- Incorrect endpoint
- Deleted resource
- Typographical error

First Checks:
- Verify the URL.
- Check the API documentation.
- Confirm the resource exists.

---

## 429 Too Many Requests

Meaning:
The client has exceeded the API rate limit.

Possible Causes:
- Too many requests
- Rate limiting policy

First Checks:
- Wait before retrying.
- Review the API rate limits.

---

## 500 Internal Server Error

Meaning:
An unexpected server error occurred.

Possible Causes:
- Server outage
- Application bug
- Database issue

First Checks:
- Check the status page.
- Review server logs (if available).
- Escalate to engineering if necessary.

---

# Support Engineer Checklist

Before escalating an API issue:

- Confirm the endpoint.
- Verify authentication.
- Check permissions.
- Review request headers.
- Validate request payload.
- Reproduce the issue.
- Collect timestamps and request IDs.