# cybersecurity-task5-wireshark
# Task 5 - Wireshark Network Traffic Capture

## Objective
Capture and analyze live network traffic using Wireshark.

## Protocols Identified
1. **DNS** - Domain name resolution (e.g., google.com → IP)
2. **ICMP** - Ping requests/replies to 8.8.8.8 and google.com
3. **TLS** - Encrypted HTTPS traffic from visiting google.com and youtube.com

## Traffic Generated
- Browsed google.com and youtube.com (HTTPS/TLS)
- Ran ping 8.8.8.8 and ping google.com (ICMP)

## Files
- task5-capture.pcapng → Full packet capture
- Screenshots showing DNS, ICMP, TLS, and overall traffic

Task completed on: 20 November 2025  
Wireshark Version: 4.6.1

## Interview Questions Answers

1. **What is Wireshark used for?**  
   Wireshark is a network packet analyzer used for troubleshooting, security analysis, and learning network protocols.

2. **What is a packet?**  
   A packet is a small unit of data sent over a network containing header (control info) and payload (actual data).

3. **How to filter packets in Wireshark?**  
   Type filters like `dns`, `icmp`, `tls`, `ip.addr == 8.8.8.8` in the filter bar and press Enter.

4. **Difference between TCP and UDP?**  
   TCP is reliable and connection-oriented; UDP is faster but unreliable (no guaranteed delivery).

5. **What is a DNS query packet?**  
   A packet sent to resolve a domain name (e.g., google.com) to an IP address using UDP port 53.

6. **How does packet capture help in troubleshooting?**  
   It reveals actual network behavior, errors, delays, packet loss, and malicious activity.

7. **What is a protocol?**  
   A standard set of rules for communication between devices (e.g., HTTP, DNS, TCP).

8. **Can Wireshark decrypt encrypted traffic?**  
   No, not without the private SSL/TLS keys. Normal HTTPS traffic remains encrypted in Wireshark.
