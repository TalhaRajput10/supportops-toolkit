# HTTP Status Codes

## What are HTTP Status Codes?

HTTP status codes are responses sent by a server to indicate whether a client's request was successful or if an error occurred.

---

# 2xx - Success

## 200 OK

The request was successful.

Example:
A user successfully retrieves their profile information.

---

## 201 Created

A new resource was successfully created.

Example:
A new customer account is registered.

---

# 4xx - Client Errors

## 400 Bad Request

The request contains invalid or missing information.

Possible Causes:
- Missing required fields
- Invalid request format
- Incorrect parameters

---

## 401 Unauthorized

The request lacks valid authentication credentials.

Possible Causes:
- Expired access token
- Invalid API key
- Missing Authorization header

---

## 403 Forbidden

The server understands the request but refuses to authorize it.

Possible Causes:
- Insufficient permissions
- Restricted resource
- Account does not have access

---

## 404 Not Found

The requested endpoint or resource does not exist.

Possible Causes:
- Incorrect URL
- Deleted resource
- Typographical error

---

## 429 Too Many Requests

The client has exceeded the API rate limit.

Possible Causes:
- Too many API requests in a short time
- Rate limiting enabled

---

# 5xx - Server Errors

## 500 Internal Server Error

An unexpected error occurred on the server.

Possible Causes:
- Application bug
- Database failure
- Unexpected server exception

---

| Status Code | Meaning | Common Cause | First Thing to Check |
|-------------|---------|--------------|----------------------|
| 200 | OK | Successful request | Verify returned data |
| 400 | Bad Request | Invalid request | Request body and parameters |
| 401 | Unauthorized | Authentication failed | API key or access token |
| 403 | Forbidden | Permission denied | User role and permissions |
| 404 | Not Found | Incorrect URL or missing resource | Check the endpoint or URL |
| 429 | Too Many Requests | Rate limit exceeded | Wait and retry later |
| 500 | Internal Server Error | Server issue | Check logs or escalate |



# Summary

Understanding HTTP status codes helps Technical Support Engineers identify whether an issue is related to the client request, authentication, permissions, missing resources, or server failures.