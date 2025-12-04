# 🔐 Security

---

## 1. Authentication vs Authorization

### High-Level Guidance
Authentication verifies **who you are**, while authorization controls **what you are allowed to do**.

### What to Know
- Authentication: login, identity validation
- Authorization: roles, permissions, access control
- Common mistake: mixing the two concepts

### Practical Usage
- JWT for authentication
- Role-based access control (RBAC) for authorization

---

## 2. Spring Security

### High-Level Guidance
Framework for securing Spring applications at the transport and application layers.

### What to Know
- Security filter chain
- `AuthenticationManager`
- `UserDetailsService`
- Password encoding (`BCrypt`)
- JWT-based authentication
- Method-level security (`@PreAuthorize`)

---

## 3. Cross-Site Scripting (XSS)

### High-Level Guidance
Injection of malicious scripts into trusted websites.

### What to Know
- Stored vs Reflected vs DOM-based XSS
- Input sanitization
- Output encoding

### Prevention
- Escaping user input
- Content Security Policy (CSP)

---

## 4. SQL Injection

### High-Level Guidance
Attacking a database by injecting malicious SQL.

### What to Know
- Happens via unvalidated user input
- Can leak or destroy data

### Prevention
- Prepared statements
- Parameterized queries
- ORM (Hibernate, JPA)

---

## 5. Cross-Site Request Forgery (CSRF)

### High-Level Guidance
Fooling an authenticated user into executing unwanted actions.

### What to Know
- Exploits trust in browser cookies
- Common in web apps with sessions

### Prevention
- CSRF tokens
- Same-site cookies
- Disabling CSRF only for stateless JWT APIs

---

## 6. OAuth 2.0 vs SAML

### High-Level Guidance
Protocols for delegated authentication and single sign-on (SSO).

### OAuth 2.0
- Token-based
- Used for APIs and modern mobile/web apps
- JSON-based (JWT)

### SAML
- XML-based
- Common in enterprise SSO
- More verbose and heavyweight

---

## 7. OWASP

### High-Level Guidance
Global organization focused on web application security.

### What to Know
- OWASP Top 10:
  - Injection
  - Broken Authentication
  - Security Misconfiguration
  - Sensitive Data Exposure
  - XSS
  - CSRF
  - Insecure Deserialization

### Practical Usage
- Security audit checklist
- API penetration testing guidance

---

## 8. Security Best Practices

### Application Level
- Always hash passwords (`BCrypt`)
- Validate and sanitize all inputs
- Use HTTPS everywhere
- Least privilege principle

### API Level
- JWT expiration + refresh
- Rate limiting
- API gateway protection

### Infrastructure Level
- Secrets management (Vault, env vars)
- Network segmentation
- WAFs and firewalls

---
