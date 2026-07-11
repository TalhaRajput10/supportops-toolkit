# Testing a GET Request in Postman

## Objective

Learn how to send a GET request using Postman and interpret the response.

---

## Endpoint

https://jsonplaceholder.typicode.com/users

---

## HTTP Method

GET

---

## Steps

1. Open Postman.
2. Create a new HTTP request.
3. Select the **GET** method.
4. Enter the endpoint URL.
5. Click **Send**.

---

## Expected Response

A JSON array containing user information.

Example:

```json
[
  {
    "id": 1,
    "name": "Leanne Graham",
    "email": "Sincere@april.biz"
  }
]
```

---

## What to Verify

- Status Code: 200 OK
- Response Time
- Response Body
- Headers

---

## Common Issues

### 404 Not Found

Verify the endpoint URL.

### 401 Unauthorized

Check authentication credentials.

### 500 Internal Server Error

Retry the request and check the API status.

---

## Skills Demonstrated

- API Testing
- Postman
- HTTP Methods
- JSON Response Analysis