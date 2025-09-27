# Applied Crypto — Hands-On

**Goal:** Build practical understanding of TLS, certificates, and secure cryptographic use in web applications.

**Prerequisites**
- Lab web server (Apache/Nginx) configured with TLS
- Tools: openssl CLI, browser devtools, Wireshark (optional)

**Exercises**
1. **Inspect TLS handshake**
   - Capture a TLS handshake and examine the certificate chain (CN, SAN, issuer, validity).
   - Identify the negotiated cipher suite and key exchange method.

2. **Certificate management**
   - Configure AutoSSL or Let's Encrypt (certbot) for a lab domain.
   - Observe certificate file locations and renewal behavior.

3. **Password storage & hashing**
   - Compare use of secure password hashing (bcrypt/argon2) versus plain hashing (SHA-256) in a small demo.
   - Discuss salting, KDFs, and why modern KDFs are necessary.

**Deliverable**
- Short report: findings from TLS inspection, recommended cipher suites to disable, and password storage best practices.

**Safety**
- Do not attempt to break cryptographic primitives in real environments. Focus on configuration and detection.
