# Web Forensics — Hands-On

**Goal:** Collect evidence related to web incidents, construct timelines from logs, and perform basic artifact analysis.

**Prerequisites**
- Lab web server with access logs (Apache/Nginx), application logs, and system logs
- Tools: grep, awk, sleuthkit (optional), timeline builders

**Exercises**
1. **Collect and preserve logs**
   - Gather access logs, error logs, authentication logs, and application logs for a test incident.
   - Create an archived copy with checksums for integrity verification.

2. **Construct an event timeline**
   - Correlate entries across logs to build a timeline: request → authentication → database action → error.
   - Identify the likely initial vector and timeline of escalation.

3. **Artifact analysis**
   - Extract suspicious request URIs, user-agents, and originating IPs.
   - If available, correlate with PCAP to confirm payloads and flows.

**Deliverable**
- Incident timeline and a short analytic report listing indicators of compromise and suggested detection improvements.

**Best practices**
- Preserve originals; perform analysis on copies. Document chain-of-custody even in lab scenarios.
