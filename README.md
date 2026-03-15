# Task 1: Basic Network Scanning with Nmap

## Objective
To perform a network scan on a target machine to identify open ports and active services.

## Tool Used
* **Nmap 7.95** (via Zenmap GUI)
* **Target:** scanme.nmap.org

## Results Summary
The scan identified the following open ports:
* **Port 22/tcp (ssh):** Used for secure remote login.
* **Port 80/tcp (http):** Used for unencrypted web traffic.

## Significance
Identifying open ports is the first step in a security assessment. Open ports like 22 and 80 represent the 'attack surface' of a server and must be monitored for vulnerabilities.