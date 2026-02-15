# AdBlock-via-DNS
📌 Project Overview
This project demonstrates the implementation of network-level ad-blocking using DNS Sinkholing. By utilizing the AdGuard DNS (94.140.14.14), this setup filters out advertisements, trackers, and malware domains before they reach the end-user device, improving both network security and bandwidth efficiency.

🚀 Deployment Methods
Network-Wide: Configured via DHCP Option 6 on the Home Gateway/Router to protect all connected devices (IoT, Smart TVs, PCs).

Mobile/Remote: Implemented via DNS-over-TLS (DoT) using the Private DNS feature on Android/iOS for protection over both Wi-Fi and Cellular data.

🛡️ Security Considerations
Privacy: Shifting DNS queries to a third-party provider requires encrypted protocols (DoT/DoH) to prevent ISP snooping.

Redundancy: Secondary DNS (e.g., 1.1.1.1) is recommended to avoid a single point of failure.

Integrity: Use of DNSSEC to mitigate DNS poisoning and unauthorized redirection.
