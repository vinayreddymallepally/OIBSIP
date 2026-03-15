# Task 4: Research Report on Common Network Security Threats

## Introduction
As networks become more complex, they also become more vulnerable to a variety of cyber attacks. This report outlines three common network security threats: Denial of Service (DoS), Man-in-the-Middle (MITM) attacks, and Spoofing. It covers how they work, their impact, and how to mitigate them.

---

## 1. Denial of Service (DoS) & Distributed Denial of Service (DDoS)
### How it Works
A DoS attack attempts to exhaust the resources of a network, application, or system so that legitimate users cannot access it. Attackers achieve this by flooding the target with excessive requests (e.g., ICMP floods or SYN floods). A DDoS attack uses a botnet (multiple compromised machines) to amplify the attack.
### Impact
* **Downtime:** Websites and services go offline, preventing business operations.
* **Financial Loss:** E-commerce sites lose revenue for every minute of downtime.
### Real-World Example
In 2018, GitHub experienced a massive DDoS attack peaking at 1.35 Tbps, which took the platform offline for several minutes.
### Mitigation & Prevention
* **Rate Limiting:** Restricting the number of requests a server accepts over a specific timeframe.
* **Traffic Scrubbing:** Using cloud services (like Cloudflare or AWS Shield) to filter out malicious traffic before it hits the server.

---

## 2. Man-in-the-Middle (MITM) Attacks
### How it Works
In a MITM attack, the attacker secretly intercepts and relays communications between two parties who believe they are directly communicating. This often happens on unsecured public Wi-Fi networks using techniques like ARP spoofing.
### Impact
* **Data Theft:** Attackers can steal login credentials, credit card numbers, and session cookies.
* **Data Manipulation:** Attackers can alter messages or transactions in transit.
### Real-World Example
An attacker sets up a fake Wi-Fi hotspot at a coffee shop named "Free Public Wi-Fi." When users connect, the attacker intercepts all their unencrypted browsing data.
### Mitigation & Prevention
* **Encryption:** Mandating HTTPS/SSL for all web traffic so intercepted data is unreadable.
* **Virtual Private Networks (VPNs):** Using VPNs encrypts the entire internet connection, protecting data even on public networks.

---

## 3. Spoofing Attacks
### How it Works
Spoofing involves an attacker masquerading as a trusted entity to gain access to a system or deceive a user. Common types include IP Spoofing (faking the source IP address) and DNS Spoofing (redirecting a domain to a fake IP).
### Impact
* **Unauthorized Access:** Bypassing IP-based authentication.
* **Malware Distribution:** Tricking users into downloading malicious payloads from fake domains.
### Real-World Example
In a DNS spoofing attack, a user types "mybank.com" but is secretly redirected to the attacker's fake website, where they unknowingly type in their username and password.
### Mitigation & Prevention
* **Packet Filtering:** Configuring firewalls to block packets with mismatched or suspicious source IP addresses.
* **DNSSEC:** Implementing Domain Name System Security Extensions to authenticate DNS responses.

---

## Conclusion
Network security requires a layered defense strategy. By understanding the mechanics of DoS, MITM, and Spoofing attacks, security analysts can implement proper encryption, traffic monitoring, and access controls to secure organizational infrastructure.
