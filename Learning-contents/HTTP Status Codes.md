
# 🌐 HTTP Status Codes – Daily Learning (17 June 2025)

## 📘 What Are HTTP Status Codes?
HTTP status codes are **3-digit responses** from the server that indicate the outcome of a client’s request to the server.

---

## 📊 Categories and Common Status Codes

---

### 🔵 1xx – Informational Responses
These codes indicate that the **request was received** and the process is **continuing**.

| Code | Meaning |
|------|---------|
| 100  | Continue – Client should continue with request |
| 101  | Switching Protocols – Server is switching protocols |
| 102  | Processing – Request is being processed (WebDAV) |
| 103  | Early Hints – Preloads resources before final response |
| 122  | Request-URI too long (non-standard, used by IE) |

---

### 🟢 2xx – Success
These indicate that the **request was successfully received**, understood, and accepted.

| Code | Meaning |
|------|---------|
| 200  | OK – Standard response for success |
| 201  | Created – Resource created successfully |
| 202  | Accepted – Request accepted but not completed |
| 203  | Non-Authoritative Information – Returned meta info may be from a third party |
| 204  | No Content – Successful but no body returned |
| 205  | Reset Content – Tells client to reset the document view |
| 206  | Partial Content – Used for range requests |

---

### 🟡 3xx – Redirection
These codes indicate that **further action is needed** to complete the request.

| Code | Meaning |
|------|---------|
| 300  | Multiple Choices – Multiple options for the resource |
| 301  | Moved Permanently – Resource moved to new URL |
| 302  | Found – Temporary redirection |
| 303  | See Other – Get the resource at another URI |
| 304  | Not Modified – Use cached version |
| 307  | Temporary Redirect – Same method should be used |
| 308  | Permanent Redirect – Method preserved like 301 |

---

### 🔴 4xx – Client Errors
The request **contains bad syntax** or **cannot be fulfilled** by the server.

| Code | Meaning |
|------|---------|
| 400  | Bad Request – Invalid request format |
| 401  | Unauthorized – Authentication required |
| 403  | Forbidden – Access denied |
| 404  | Not Found – Resource not found |
| 405  | Method Not Allowed – Request method is not supported |
| 408  | Request Timeout – Server timed out waiting |
| 409  | Conflict – Resource conflict (e.g., duplicate entry) |
| 410  | Gone – Resource no longer available |
| 429  | Too Many Requests – Rate limit exceeded |

---

### 🔴 5xx – Server Errors
These codes indicate that the **server failed** to fulfill a **valid request**.

| Code | Meaning |
|------|---------|
| 500  | Internal Server Error – Generic server error |
| 501  | Not Implemented – Server does not support the functionality |
| 502  | Bad Gateway – Invalid response from upstream |
| 503  | Service Unavailable – Server overloaded or down |
| 504  | Gateway Timeout – Upstream server timed out |
| 505  | HTTP Version Not Supported |
| 507  | Insufficient Storage – Server is out of storage space (WebDAV) |
| 511  | Network Authentication Required – Login required to access network |

---

## 🧠 Pro Tip:
When building APIs:
- Return `201 Created` after POST requests that create data.
- Use `204 No Content` when the request succeeded but nothing needs to be returned.
- Always return `404` for missing resources and `500` for server crashes in production.
