# FUTURE_CS_03  
## API Security Risk Analysis

---

## 🎯 Objective

The objective of this task is to perform a read-only API security assessment on a public demo API to identify common API security risks such as unauthenticated access, excessive data exposure, and missing security controls.

---

## 🔎 API Selected

**ReqRes (Public Test API)**  
https://reqres.in  
Base URL: https://reqres.in/api  

This API was selected because it is publicly accessible, designed for testing purposes, and simulates real-world authentication and user management features.

---

## 🛠 Tools Used

- Postman (API Testing)  
- Web Browser (Endpoint Verification)  
- Kali Linux Terminal (Header Inspection using curl)  
- GitHub (Project Documentation)

---

## 🧪 Endpoints Tested

- `/api/users`
- `/api/users/2`
- `/api/login`
- `/api/register`

---

## 🔍 Security Findings

### ⚠️ Unauthenticated Endpoint Access
Certain endpoints were accessible without authentication.

**Risk Level:** Medium

---

### ⚠️ Excessive Data Exposure
User-related endpoints return complete user objects without role-based restrictions.

**Risk Level:** Medium

---

### ⚠️ Missing Rate Limiting Indicators
No visible rate-limiting headers were observed during testing.

**Risk Level:** Medium

---

### ⚠️ Public Demo Data
The API contains demo data only and does not expose real sensitive information.

**Risk Level:** Low

---

## 🛡️ Recommendations

- Implement strict authentication and authorization controls.
- Limit unnecessary data fields in API responses.
- Enable rate limiting to prevent abuse.
- Apply proper input validation.
- Configure appropriate security headers.

---

## ✅ Conclusion

This project demonstrates a beginner-level API security assessment conducted using safe and ethical testing practices. The analysis identifies common API security risks and provides remediation recommendations based on standard security principles.
