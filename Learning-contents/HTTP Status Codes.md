## **HTTP Status Codes**

### **✅ What are HTTP Status Codes?**

HTTP status codes are **three-digit codes** returned by a server in response to a client's request. They help indicate whether a specific HTTP request has been successfully completed or if there was an error.

---

### **📊 HTTP Status Code Categories**

| Code Range | Category | Description |
| ----- | ----- | ----- |
| 1xx | Informational | Request received, continuing process |
| 2xx | Success | Request successfully received and processed |
| 3xx | Redirection | Further action needed to complete the request |
| 4xx | Client Error | Request has bad syntax or cannot be fulfilled |
| 5xx | Server Error | Server failed to fulfill a valid request |

---

### **🔢 Common Status Codes and Meanings**

#### **✅ 2xx: Success**

* **200 OK** – Standard response for successful HTTP requests.

* **201 Created** – Request has been fulfilled and new resource is created.

* **204 No Content** – Request succeeded, but no content to return.

#### **🔁 3xx: Redirection**

* **301 Moved Permanently** – Resource has been permanently moved.

* **302 Found** – Resource temporarily moved to another URL.

* **304 Not Modified** – Cached version is still valid; no need to resend.

#### **❌ 4xx: Client Errors**

* **400 Bad Request** – Malformed request syntax or invalid request.

* **401 Unauthorized** – Authentication required or failed.

* **403 Forbidden** – Server understood but refuses to authorize.

* **404 Not Found** – Resource not found at the requested URL.

* **409 Conflict** – Request conflicts with current state of the server.

#### **🛠️ 5xx: Server Errors**

* **500 Internal Server Error** – Generic server error.

* **502 Bad Gateway** – Invalid response from the upstream server.

* **503 Service Unavailable** – Server is currently unavailable (overload or maintenance).

