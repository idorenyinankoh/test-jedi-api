**API documentation** with full CRUD operations

---

# 📘 **Sample API Documentation**

### **Base URL**
```
https://3a0bfe56-7258-4955-9f23-252bddaf0879.mock.pstmn.io
```

---

## 📌 **Resource: Users**

---

### 🔍 Get User  
**Method:** `GET`  
**Endpoint:** `/users/{id}`  

**Sample Request:**
```
GET {{baseUrl}}/v1/users/{{id}}
```

**Response:**
```json
{
  "id": "u12345",
  "first_name": "Jane",
  "last_name": "Doe",
  "email": "jane.doe@example.com",
  "role": "admin",
  "created_at": "2025-04-11T10:00:00Z"
}
```

---

### ✅ Create User  
**Method:** `POST`  
**Endpoint:** `/v1/users`  

**Request Payload:**
```json
{
  "first_name": "Jane",
  "last_name": "Doe",
  "email": "idy.doe@example.com",
  "role": "admin"
}
```

**Response:**
```json
{
  "id": "u12345",
  "first_name": "Jane",
  "last_name": "Doe",
  "email": "jane.doe@example.com",
  "role": "admin",
  "created_at": "2025-04-11T10:00:00Z"
}
```

---

### ✏️ Update Entire User Info  
**Method:** `PUT`  
**Endpoint:** `/v1/users/{id}`  

**Request Payload:**
```json
{
  "first_name": "Janet",
  "last_name": "Doe",
  "email": "janet.doe@example.com",
  "role": "editor"
}
```

**Response:**
```json
{
  "id": "u12345",
  "first_name": "Janet",
  "last_name": "Doe",
  "email": "janet.doe@example.com",
  "role": "editor",
  "updated_at": "2025-04-11T12:30:00Z"
}
```

---

### 🛠️ Partially Update User Info  
**Method:** `PATCH`  
**Endpoint:** `/v1/users/{id}`  

**Request Payload:**
```json
{
  "role": "viewer"
}
```

**Response:**
```json
{
  "id": "u12345",
  "first_name": "Janet",
  "last_name": "Doe",
  "email": "janet.doe@example.com",
  "role": "viewer",
  "updated_at": "2025-04-11T13:00:00Z"
}
```

---

### ❌ Delete a User  
**Method:** `DELETE`  
**Endpoint:** `/v1/users/{id}`  

**Response:**
```json
{
  "message": "User deleted successfully",
  "id": "u12345"
}
```

---
