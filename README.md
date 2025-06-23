# network-scan-task
Task 1 – Local Network Port Scanning with Nmap and Wireshark
Objective:
Discover open ports on devices in my local network using Nmap and analyze traffic using Wireshark to understand network exposure and potential vulnerabilities.

Tools Used:

Nmap (Command-line TCP SYN scan)

Wireshark (Packet capture and analysis)

Steps Taken:

Installed Nmap and Wireshark on Windows.

Identified my local IP range using ipconfig or System Information.

Performed a scan using:
nmap -sS 192.168.1.0/24 -oN 
scan-results.txt
Simultaneously captured traffic using Wireshark on my active network interface.

Applied the filter: tcp.flags.syn == 1 to view SYN packets used in the scan.

Analyzed responses:

SYN-ACK = port open

RST = port closed

No response = filtered

Saved:

Nmap scan as .txt

Wireshark capture as .pcapng

Findings:

Open ports on local devices included 22 (SSH), 80 (HTTP), and 445 (SMB)

SMB service exposed = potential security risk

Recommendation: disable unused services and secure access via firewall

Screenshots and Files:
![d47b58ac-1ba4-41af-b20e-70f947c4bbb9](https://github.com/user-attachments/assets/a06ba27e-77ed-4882-a726-d1c660d5df7d)


![fb0c0082-86ab-4aa2-99ec-716518c7d087](https://github.com/user-attachments/assets/1a99b415-a52d-47c7-a97f-156f2a4ebac4)

![a3de96b2-f9bc-416a-8fa4-f55eebf41710](https://github.com/user-attachments/assets/bc220c9c-e3ba-4f40-911b-eec7f59b58a3)

thank you
