# Task 10: Security Assessment Report

## 1. Introduction
This report summarizes a security assessment performed on network assets and traffic. The objective was to identify potential vulnerabilities using industry-standard tools and provide actionable recommendations to improve the security posture.

---

## 2. Methodology
The assessment was conducted using the following tools:
* **Nmap:** For network discovery and port scanning.
* **Wireshark:** For deep packet analysis and traffic monitoring.

---

## 3. Vulnerability Findings

### A. Unencrypted Services (Critical)
* **Evidence:** During Task 8, Wireshark captured raw HTTP traffic (GET requests).
* **Risk:** Data transmitted via HTTP is sent in plain text. An attacker performing a Man-in-the-Middle (MITM) attack can intercept sensitive information such as session cookies or login credentials.
* **Recommendation:** Enforce HTTPS (TLS 1.3) across all web platforms.

### B. Open Ports and Attack Surface (Medium)
* **Evidence:** The Nmap scan in Task 1 revealed open ports (Port 22, Port 80).
* **Risk:** While Port 22 (SSH) is necessary for remote management, Port 80 (HTTP) increases the attack surface unnecessarily if not strictly required.
* **Recommendation:** Implement a firewall to restrict Port 22 access to specific IP addresses and close Port 80 in favor of Port 443 (HTTPS).

---

## 4. Proposed Security Mitigation Plan
1. **Encryption:** Transition all legacy HTTP services to HTTPS.
2. **Access Control:** Utilize Key-Based Authentication for SSH instead of passwords.
3. **Monitoring:** Deploy an Intrusion Detection System (IDS) to monitor for suspicious spikes in traffic (DoS/DDoS protection).

---

## 5. Conclusion
The assessment revealed that while the basic network infrastructure is functional, it is vulnerable to interception and unauthorized access due to unencrypted traffic. Implementing the recommendations above will significantly reduce the organizational risk.

**Assessor:** [MALLEPALLY SAI VINAY]  
**Date:** March 2026
