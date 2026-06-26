# 📡 Task 8 - Capture Network Traffic with Wireshark

## Oasis Infobyte Cyber Security Internship

---

# 📌 Internship Information

| Attribute          | Details                                  |
| ------------------ | ---------------------------------------- |
| Internship Program | Oasis Infobyte Cyber Security Internship |
| Task Number        | Task 8                                   |
| Task Title         | Capture Network Traffic with Wireshark   |
| Domain             | Cyber Security                           |
| Intern Name        | Tarak Ram                                |
| Duration           | June 2026 - July 2026                    |

---

# 📖 Project Overview

Network traffic analysis is one of the most important activities in cybersecurity. Monitoring and analyzing network packets helps security professionals detect suspicious activities, troubleshoot network issues, and investigate cyber incidents.

In this project, Wireshark was used to capture and analyze network traffic generated on a local network. Various network protocols such as TCP, DNS, HTTP, and HTTPS were examined to understand how devices communicate over a network.

---

# 🌐 About Wireshark

Wireshark is a free and open-source network protocol analyzer widely used by network administrators, cybersecurity analysts, ethical hackers, and security researchers.

It captures packets traveling across a network and provides detailed information about each packet, including:

* Source IP Address
* Destination IP Address
* Protocol Used
* Packet Length
* Port Numbers
* Packet Payload

Wireshark is commonly used for:

* Network Troubleshooting
* Security Monitoring
* Malware Analysis
* Incident Response
* Protocol Analysis
* Performance Analysis

Official Website:

https://www.wireshark.org/

---

# 🎯 Objectives

The primary objectives of this task are:

* To install and configure Wireshark.
* To capture live network packets.
* To observe communication between devices.
* To filter captured packets using protocol filters.
* To analyze network traffic.
* To understand various network protocols.
* To gain practical experience in packet analysis.

---

# 🛠️ Tools and Technologies Used

| Tool/Technology          | Purpose                                   |
| ------------------------ | ----------------------------------------- |
| Wireshark                | Capturing and analyzing network traffic   |
| Windows Operating System | Execution environment                     |
| Web Browser              | Generating network traffic                |
| GitHub                   | Project documentation and version control |

---

# ⚙️ Environment Setup

## Step 1: Install Wireshark

1. Download Wireshark from the official website.
2. Execute the installer.
3. Select default installation options.
4. Install Npcap when prompted.
5. Complete the installation.

Official Download Link:

https://www.wireshark.org/download.html

---

# 🚀 Procedure

## Step 1: Launch Wireshark

After successful installation, Wireshark was launched.

The application displayed available network interfaces such as:

* Wi-Fi
* Ethernet

The active network interface connected to the Internet was selected.

---

## Step 2: Start Packet Capture

The active network adapter was double-clicked to begin packet capturing.

Wireshark immediately started capturing incoming and outgoing packets from the local network.

---

## Step 3: Generate Network Traffic

To generate traffic, several websites were accessed through a web browser.

Examples:

* https://www.google.com
* https://www.youtube.com
* http://neverssl.com

Browsing activity generated multiple packets for analysis.

---

## Step 4: Stop Packet Capture

After capturing packets for a few minutes, packet capturing was stopped by clicking the **Stop Capture** button.

---

## Step 5: Apply Packet Filters

To simplify analysis, protocol filters were applied.

### HTTP Filter

```text
http
```

### TCP Filter

```text
tcp
```

### DNS Filter

```text
dns
```

Filtering allowed only specific protocol packets to be displayed.

---

## Step 6: Analyze Captured Packets

Individual packets were selected for detailed inspection.

The following information was analyzed:

* Source Address
* Destination Address
* Protocol Type
* Source Port
* Destination Port
* Packet Size
* Packet Payload

---

## Step 7: Save Packet Capture

The captured traffic was saved as:

```text
wireshark_capture.pcap
```

This file contains all captured network packets and can be reopened later for analysis.

---

# 📊 Observed Network Protocols

During packet analysis, the following protocols were observed:

| Protocol | Description                                   |
| -------- | --------------------------------------------- |
| TCP      | Provides reliable communication between hosts |
| DNS      | Resolves domain names into IP addresses       |
| HTTP     | Transfers web pages between client and server |
| HTTPS    | Secure version of HTTP using encryption       |
| TLS      | Provides secure encrypted communication       |
| ARP      | Maps IP addresses to MAC addresses            |

---

# 🔍 Sample Packet Analysis

## Packet 1

**Protocol:** TCP

**Purpose:** Establishes communication between devices.

**Observation:** Used for reliable data transmission.

---

## Packet 2

**Protocol:** DNS

**Purpose:** Resolves domain names into IP addresses.

**Observation:** Generated when visiting websites.

---

## Packet 3

**Protocol:** HTTPS/TLS

**Purpose:** Secure communication over the Internet.

**Observation:** Most modern websites use encrypted HTTPS traffic.

---

# 📷 Screenshots Included

The following screenshots are included in this repository:

1. Wireshark Installation/Home Screen.
2. Live Packet Capture.
3. Filtered Packet View.
4. Detailed Packet Analysis.
5. Saved PCAP File.

All screenshots are stored in the **screenshots** folder.

---

# 📂 Repository Structure

```text
Task8_Capture_Network_Traffic/
│
├── wireshark_capture.pcap
├── analysis_report.md
├── README.md
└── screenshots/
    ├── Screenshot_1_Wireshark_Installation.png
    ├── Screenshot_2_Live_Capture.png
    ├── Screenshot_3_HTTP_Filter.png
    ├── Screenshot_4_Packet_Details.png
    └── Screenshot_5_PCAP_File.png
```

---

# 🧠 Learning Outcomes

After completing this task, the following skills were acquired:

* Understanding of packet capture techniques.
* Knowledge of network communication processes.
* Ability to use Wireshark for packet analysis.
* Understanding of common network protocols.
* Practical experience in network traffic monitoring.

---

# 🔐 Security Considerations

Packet capturing should only be performed on networks that you own or are authorized to analyze.

Unauthorized interception of network traffic may violate organizational policies and legal regulations.

---

# ✅ Conclusion

This project successfully demonstrated the process of capturing and analyzing network traffic using Wireshark. The captured packets provided valuable insights into network communication and protocol behavior.

Wireshark proved to be an essential cybersecurity tool for network monitoring, troubleshooting, and security analysis. Understanding network traffic is fundamental for detecting anomalies, investigating incidents, and strengthening overall network security.

---

# 👨‍💻 Author

**Tarak Ram**

Cyber Security Intern

Oasis Infobyte

