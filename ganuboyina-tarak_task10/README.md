# Task 10: Detailed Security Assessment Report for a Network

## Objective

The objective of this task was to perform a security assessment on a local network using network scanning and traffic analysis tools. The assessment involved identifying open ports, analyzing network traffic, detecting active services, and evaluating potential security risks.

---

## Tools Used

* Nmap 7.99
* Wireshark
* Windows 11 Pro
* Command Prompt (CMD)
* GitHub

---

## Task Execution

### Step 1: Perform Network Scanning using Nmap

A network scan was performed on the local machine to identify open ports and active services.

The following command was executed:

```
nmap -A localhost
```

The scan provided detailed information regarding:

* Open Ports
* Running Services
* Service Versions
* Operating System Information

---

### Step 2: Save Nmap Scan Results

The scan results were saved in a text file named:

```
nmap_results.txt
```

This file contains the complete output of the Nmap scan.

---

### Step 3: Capture Network Traffic using Wireshark

Wireshark was launched and the active network interface was selected.

Live network traffic was captured while browsing websites and accessing online services.

---

### Step 4: Apply Packet Filters

To analyze specific traffic, the following filters were applied:

```
http
tcp
dns
```

These filters helped isolate packets related to web communication and domain name resolution.

---

### Step 5: Analyze Captured Traffic

Captured packets were analyzed to observe:

* Source and Destination IP Addresses
* Protocol Types
* Port Numbers
* Packet Length
* Communication Patterns

---

## Assessment Findings

The assessment identified multiple active services and network protocols.

### Nmap Findings

* Several TCP ports were found to be open.
* Microsoft services such as SMB and RPC were active.
* SQL Server-related services were detected.
* Web services were running on the system.

### Wireshark Findings

* DNS queries were observed during web browsing.
* TCP sessions established communication between hosts.
* HTTPS traffic provided secure encrypted communication.
* Multiple network protocols were identified.

---

## Security Analysis

### Open Ports

Open ports increase the attack surface of a system. Services running on these ports should be monitored and secured properly.

### SMB Services

SMB services should be restricted and regularly updated because attackers frequently target these services.

### Web Services

Web services should use secure communication protocols such as HTTPS.

### Network Monitoring

Continuous monitoring of network traffic helps detect suspicious activities and potential threats.

---

## Risk Assessment

| Risk                        | Severity |
| --------------------------- | -------- |
| Unnecessary Open Ports      | Medium   |
| Exposed SMB Services        | High     |
| Unmonitored Network Traffic | Medium   |
| Outdated Services           | High     |

---

## Recommendations

* Regularly monitor network traffic.
* Disable unused services and ports.
* Keep software and operating systems updated.
* Use firewalls to restrict unauthorized access.
* Enable intrusion detection and prevention mechanisms.
* Conduct periodic security assessments.

---

## Key Observations

* The local system was active and reachable.
* Multiple services were running on the system.
* Encrypted traffic was observed.
* Network communication patterns were successfully analyzed.

---

## Learning Outcomes

Through this task, I gained practical experience in:

* Performing network security assessments.
* Using Nmap for service discovery.
* Capturing packets using Wireshark.
* Analyzing network communication.
* Identifying security risks and vulnerabilities.
* Documenting assessment findings.

---

## Files Included

Task10_Network_Security_Assessment/
│
├── README.md
├── network_security_assessment.md
├── nmap_results.txt
├── wireshark_capture.pcap
└── screenshots/

---

## Conclusion

This task successfully demonstrated the process of conducting a basic network security assessment using Nmap and Wireshark. The assessment identified active services, analyzed network traffic, and highlighted potential security concerns.

Regular security assessments are essential for maintaining a secure network environment and reducing cybersecurity risks.

---

### Author

**Tarak Ram**

Security Analyst Intern

Oasis Infobyte

