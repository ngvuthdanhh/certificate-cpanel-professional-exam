# Privilege Escalation (Web Context) — Hands-On

**Goal:** Identify configuration mistakes in web apps and servers that could enable privilege escalation, and learn how to remediate them.

**Prerequisites**
- Lab web application and server (isolated VM)
- A non-privileged user account for auditing

**Exercises**
1. **File permissions & upload handling**
   - Audit upload directories for world-writable permissions and executable flags.
   - Propose controls: deny execute in upload directories, validate and sanitize filenames, store uploads outside web root.

2. **Sudoers & privileged commands**
   - Review `/etc/sudoers` and included files for NOPASSWD or wildcard entries.
   - Document any allowed commands that could be abused to gain a shell.

3. **Credential & secret handling**
   - Search the codebase and config for hard-coded credentials in the lab.
   - Recommend secret management practices: environment variables, vaults, and restricted config file permissions.

**Deliverable**
- Audit report listing misconfigurations, severity, and prioritized remediation steps.

**Ethics & safety**
- Do not use audit results to attack systems beyond the lab. Recommendations should always aim to harden and remediate.
