TASK-5 Capture and Analyze Network Traffic Using Wireshark

1) Task Overview: Capture live network packets using Wireshark, filter the captured traffic by protocol, and analyze at least three different protocols to understand their basic functionality in network communication.

2) Objective
Capture live network packets and identify basic protocols and traffic types

3) Tools Used
- Wireshark (for packet capture and analysis)
- Windows 11 (host machine environment)

4) Steps Followed

a. Installed Wireshark on the system.
b. Started capturing on the active network interface (Wi-Fi).
c. Generated network traffic by browsing websites.
d. Stopped capture after a minute to save relevant data.
e. Filtered traffic for different protocols including ARP, DNS, and TCP.
f. Analyzed packets to understand their structure and purpose.



5) Protocols Identified & Analysis
- (The `.pcapng` file for the analysis has been uploaded here: https://drive.google.com/file/d/13ziXgU7FyJJ5WiUPP6SQoxHTdkFZnEO2/view?usp=drivesdk

a. ARP (Address Resolution Protocol)
- Filter Used:`arp`
- Purpose: Resolves IP addresses to MAC addresses within the local network.
- Example Observation:
  - ARP request: `Who has 192.168.29.17? Tell 192.168.29.223`
  - Source MAC: `66:5b:0f:fd:73:c8` broadcasting to all devices to identify the MAC address of the target IP.
  - ![ARP](https://github.com/user-attachments/assets/43eaa4f4-9160-4510-b158-114b01050846)



b. DNS (Domain Name System)
- Filter Used: `dns`
- Purpose: Resolves domain names to IP addresses (both IPv4 and IPv6).
- Example Observation:
  - DNS query response resolving `nfsu.ac.in` with an AAAA record.
  - Protocol used: UDP over port 53.
  - ![DNS](https://github.com/user-attachments/assets/cae56341-e80b-4715-b6ab-4e73086fe2d5)




c. TCP (Transmission Control Protocol)
- Filter Used: `tcp`
- Purpose: Provides reliable, connection-oriented communication.
- Example Observation:
  - Standard TCP 3-way handshake with SYN, SYN-ACK, ACK packets.
  - Data transfer occurring over port 443 (HTTPS) and port 80 (HTTP).
  - ![TCP](https://github.com/user-attachments/assets/3bdfd640-bd38-4a57-a546-34c50d06fba0)




6) Key Learnings

- Captured and identified ARP, DNS, and TCP protocols in live network traffic.
- Understood protocol functionality in real-time scenarios:
  - ARP for LAN address resolution
  - DNS for hostname resolution
  - TCP for reliable data transmission.
- Practiced Wireshark filters to isolate and analyze specific traffic types effectively.






7) Conclusion
Successfully completed Task 5 by capturing live network traffic, analyzing three core protocols, and enhancing hands-on skills in packet analysis and protocol awareness.
