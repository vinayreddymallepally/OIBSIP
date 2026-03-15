# Task 8: Capture Network Traffic with Wireshark

## Objective
To capture and analyze local network traffic to understand packet flow and how unencrypted data is transmitted.

## Tools Used
* **Wireshark**

## Steps Performed
1. Selected the active Wi-Fi/Ethernet interface in Wireshark.
2. Initiated a live packet capture.
3. Generated unencrypted web traffic by navigating to an HTTP website.
4. Stopped the capture and applied the `http` display filter to isolate the web traffic.
5. Analyzed the `GET` request packets to observe plain-text data transmission.

## Key Findings
By filtering for HTTP traffic, I was able to observe how unencrypted protocols transmit data in plain text. This highlights the critical need for HTTPS/SSL encryption to prevent Man-in-the-Middle (MITM) attacks and data interception.

### [🎥 Click here to watch the Task 8 Demo Video](https://drive.google.com/file/d/1HYuXznRUmWFf1km3w7bnjpxOjrdjuNh4/view?usp=sharing)
