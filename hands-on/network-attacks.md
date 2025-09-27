# Network Attacks (Web Context) — Hands-On

**Goal:** Observe how network-layer attacks affect web services and learn safe detection and mitigation techniques.

**Prerequisites**
- Isolated lab network with at least one server and one client VM
- Tools: Wireshark / tcpdump, load generator (ab/hey), system monitors (top, iftop)

**Exercises**
1. **Packet capture & analysis**
   - Capture HTTP and HTTPS traffic while loading a test web app.
   - Analyze TCP handshake, HTTP request/response, and TLS handshake differences.
   - Note where sensitive data would be exposed without TLS.

2. **DoS simulation (controlled, non-destructive)**
   - Generate an increased but controlled load using a load tool.
   - Monitor CPU, memory, connection table size, and service response times.
   - Test mitigations: connection limits, rate-limiting, caching.

3. **MITM observation (theory and detection)**
   - Run a lab proxy to observe HTTP traffic; do not attempt TLS interception on production.
   - Learn to detect MITM by checking certificate chains, CN/SAN mismatches, and pinning failures.

**Deliverable**
- PCAP sample and a short analysis describing observed impacts and recommended defensive measures.

**Safety**
- Do not run attacks against networks you do not control. Keep experiments contained and reversible.
