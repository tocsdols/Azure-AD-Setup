# Azure-AD-Setup
# Created a Windows Server virtual machine in Microsoft Azure to serve as the Domain Controller for the Active Directory lab environment.

##  Objective

The objective of this project is to build a basic Intrusion Detection System (IDS) capable of detecting suspicious network activity by monitoring TCP SYN packet behavior in real time.

The project focuses on identifying potential port scanning attempts by analyzing repeated connection requests from the same IP address within a specified time window.

##  Skills Learned

- Network traffic analysis
- Packet sniffing with Scapy
- TCP/IP and SYN packet understanding
- Basic intrusion detection concepts
- Python scripting for cybersecurity
- Real-time threat monitoring
- Logging and alert generation
- Working with packet-level network data

##  Tools Used

- Python 3
- Scapy
- Npcap (Windows packet capture support)
- Command Prompt / Terminal
- VS Code (or preferred code editor)
- Git & GitHub

##  Steps Used

1. Installed Python and Scapy for packet analysis.
2. Configured packet capture support using Npcap (Windows).
3. Created a packet sniffing script using Scapy.
4. Filtered TCP packets with SYN flags enabled.
5. Stored and tracked source IP addresses sending SYN packets.
6. Implemented detection logic for repeated SYN requests within 60 seconds.
7. Generated alerts when suspicious activity exceeded the threshold.
8. Logged intrusion attempts into `scan_log.txt`.
9. Tested the IDS in a controlled environment.

##  How It Works

- The IDS monitors live TCP traffic using `Scapy`.
- If it detects more than **10 SYN packets** from the same IP within 60 seconds, it flags it as a **potential scan**.
- Detected scans are printed to the terminal **and logged into a file** named `scan_log.txt`.

**Output Example**
Terminal Output:


Intrusion Detection System is running...
[2025-06-05 15:42:11] 🚨 Port scan detected from 192.168.86.5 — SYN packets: 11


Log File (scan_log.txt):
[2025-06-05 15:42:11] 🚨 Port scan detected from 192.168.86.5 — SYN packets: 11



**Detection Logic**
This IDS specifically looks for:

TCP packets with the SYN flag, which indicates an attempt to initiate a connection.
Repeated SYNs from the same IP address are counted.
If an IP sends more than 10 SYNs in a short period, it's logged and flagged as a potential scan.



## 🎥 Project Demo

Watch the full project walkthrough and live demonstration here:

[YouTube Demo Link](https://www.youtube.com/watch?v=yJuEgMhqsNk)




## 📸 Screenshots
**Real-time network sniffing**

<img width="1190" height="594" alt="Pasted Graphic" src="https://github.com/user-attachments/assets/948d809b-b52e-4527-ad75-0a098422e59c" />
<img width="583" height="383" alt="Configuration" src="https://github.com/user-attachments/assets/860a608f-d15b-49af-93eb-25af270eed21" />



**Port scan detection via TCP SYN pattern**

<img width="655" height="417" alt="Pasted Graphic 5" src="https://github.com/user-attachments/assets/060a6cbb-6b78-49af-93f2-1751d3bbf013" />



**Log file terminal output**

 - Alerts are logged to scan_log.txt for auditing

<img width="689" height="437" alt="Pasted Graphic 6" src="https://github.com/user-attachments/assets/cdce6d42-143f-4629-8611-50355a265205" />







**Samuel — Aspiring SOC Analyst & Cybersecurity Enthusiast**


