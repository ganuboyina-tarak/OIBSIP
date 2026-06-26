# 🔍 Task 1 - Basic Network Scanning with Nmap

## 📌 Internship Details

* **Internship Program:** Oasis Infobyte Cyber Security Internship
* **Domain:** Cyber Security
* **Task Number:** Task 1
* **Task Name:** Basic Network Scanning with Nmap
* **Intern Name:** Tarak Ram

---

# 📖 Project Overview

Network scanning is one of the fundamental activities in cybersecurity. It helps security professionals identify active hosts, discover open ports, and determine the services running on a system.

In this project, a basic network scan was performed using **Nmap (Network Mapper)** on a local machine to identify open ports and associated services. The scan results were analyzed to understand the security implications of exposed services.

---

# 🎯 Objective

The primary objective of this task is to:

* Install and configure Nmap.
* Perform a basic network scan on a local machine.
* Identify open ports and running services.
* Analyze the significance of discovered ports.
* Document the findings in a professional manner.

---

# 🛠️ Tools and Technologies Used

| Tool                     | Purpose                                   |
| ------------------------ | ----------------------------------------- |
| Nmap                     | Network scanning and service discovery    |
| Command Prompt           | Executing Nmap commands                   |
| Windows Operating System | Test environment                          |
| GitHub                   | Project documentation and version control |

---

# ⚙️ Environment Setup

### Step 1: Install Nmap

1. Download Nmap from the official website.
2. Run the installer.
3. Complete the installation using default settings.

Official Website:

https://nmap.org/download.html

---

### Step 2: Verify Installation

Open Command Prompt and execute:

```bash
nmap --version
```

Successful installation displays the installed version of Nmap.

---

# 🌐 Identifying Local IP Address

To identify the local machine's IPv4 address, the following command was executed:

```bash
ipconfig
```

Example Output:

```bash
IPv4 Address . . . . . . . . . . : 192.168.1.5
```

This IP address was used as the target for the network scan.

---

# 🚀 Network Scanning Procedure

## Basic Scan

The following command was executed:

```bash
nmap 192.168.1.5
```

This command performs a basic scan of the target system and displays:

* Open Ports
* Port States
* Running Services

---

## Saving Scan Results

To save the scan results into a text file, the following command was executed:

```bash
nmap 192.168.1.5 -oN nmap_scan_results.txt
```

The output was stored in:

```text
nmap_scan_results.txt
```

---

# 📊 Sample Scan Results

| Port Number | State | Service      |
| ----------- | ----- | ------------ |
| 135         | Open  | MSRPC        |
| 139         | Open  | NetBIOS-SSN  |
| 445         | Open  | Microsoft-DS |

---

# 🔎 Analysis of Open Ports

### Port 135 (MSRPC)

* Used by Microsoft Remote Procedure Call.
* Enables communication between network applications.
* Frequently used by Windows services.

### Port 139 (NetBIOS-SSN)

* Supports file and printer sharing.
* Commonly used in Windows networking environments.

### Port 445 (Microsoft-DS)

* Used by SMB (Server Message Block).
* Responsible for file sharing and remote administration.
* Should be carefully monitored because attackers often target SMB services.

---

# 📷 Screenshots

The following screenshots have been included in this repository:

1. Nmap Installation Verification
2. Local IP Address Identification
3. Basic Network Scan Execution
4. Saved Scan Output

Screenshots are available inside the **screenshots** folder.

---

# 📂 Project Directory Structure

```text
Task1_Basic_Network_Scanning/
│
├── nmap_scan_results.txt
├── README.md
└── screenshots/
    ├── Screenshot_1_Nmap_Installation.png
    ├── Screenshot_2_IP_Address.png
    ├── Screenshot_3_Network_Scan.png
    └── Screenshot_4_Saved_Output.png
```

---

# 🛡️ Security Considerations

* Network scanning should only be performed on systems that you own or are authorized to test.
* Unauthorized scanning of third-party systems may violate legal and ethical guidelines.

---

# 🎓 Learning Outcomes

Through this task, the following concepts were learned:

* Installation and usage of Nmap.
* Basic network reconnaissance techniques.
* Identification of open ports and services.
* Interpretation of Nmap scan results.
* Importance of network enumeration in cybersecurity.

---

# ✅ Conclusion

This project successfully demonstrated the use of Nmap for performing basic network reconnaissance. The scan identified active services and open ports on the local machine. Understanding these services is essential for assessing the security posture of a system and identifying potential attack surfaces.

Nmap is a powerful tool widely used by cybersecurity professionals for network discovery, security auditing, and vulnerability assessment.

---

# 👨‍💻 Author

**Tarak Ram**

Cyber Security Intern

Oasis Infobyte

