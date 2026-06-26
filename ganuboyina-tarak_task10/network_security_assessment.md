# Network Security Assessment Report

## Executive Summary

A comprehensive network security assessment was performed on the local machine to evaluate its security posture and identify potential security risks. The assessment involved network reconnaissance, service enumeration, and network traffic analysis using industry-standard cybersecurity tools such as Nmap and Wireshark.

The primary objective of this assessment was to identify active services, analyze communication patterns, evaluate security risks associated with exposed services, and provide recommendations to improve the overall security of the system.

The assessment successfully identified multiple open ports, active network services, and various communication protocols operating within the local environment.

---

## Introduction

Network security assessments play a crucial role in modern cybersecurity practices. Organizations regularly perform security assessments to identify vulnerabilities, understand network exposure, and strengthen their overall security posture.

A network security assessment helps security professionals to:

* Identify active hosts and services.
* Discover open ports and network exposure.
* Analyze network communication.
* Detect insecure configurations.
* Evaluate potential attack surfaces.
* Recommend appropriate security controls.

This assessment was conducted within a controlled local environment to ensure ethical and authorized testing.

---

## Scope of Assessment

The assessment focused on the following components:

* Local Machine
* Open Ports
* Running Services
* Network Traffic
* Communication Protocols
* Security Risks
* Service Exposure

The assessment was restricted only to systems owned and authorized for testing.

---

## Assessment Methodology

The assessment was conducted using the following methodology.

### Phase 1: Information Gathering

Basic information about the target system was collected, including IP address identification and host availability.

---

### Phase 2: Network Scanning

Nmap was used to identify:

* Open Ports
* Running Services
* Service Versions
* Operating System Information

The following command was executed:

```text
nmap -A localhost
```

The aggressive scan option enabled service detection, operating system identification, and script scanning.

---

### Phase 3: Traffic Capture

Wireshark was used to capture live network traffic generated while browsing websites and accessing network resources.

Captured traffic included:

* TCP Traffic
* DNS Queries
* HTTP Traffic
* HTTPS Traffic
* TLS Sessions

---

### Phase 4: Traffic Analysis

Captured packets were analyzed to understand communication patterns and identify protocols in use.

Important packet attributes analyzed:

* Source Address
* Destination Address
* Source Port
* Destination Port
* Protocol Type
* Packet Length
* Packet Payload

---

### Phase 5: Risk Identification

The identified services and communication patterns were evaluated to determine possible security risks.

---

## Tools Used

| Tool                   | Purpose                                |
| ---------------------- | -------------------------------------- |
| Nmap                   | Network scanning and service detection |
| Wireshark              | Packet capture and traffic analysis    |
| Windows Command Prompt | Executing scan commands                |
| Web Browser            | Generating network traffic             |
| GitHub                 | Documentation and version control      |

---

## Nmap Scan Analysis

The Nmap scan identified multiple open TCP ports and active services running on the system.

### Commonly Observed Ports

| Port | Service              |
| ---- | -------------------- |
| 80   | HTTP                 |
| 135  | MSRPC                |
| 445  | Microsoft-DS         |
| 1433 | Microsoft SQL Server |
| 1434 | SQL Server Browser   |

### Analysis

#### Port 80 (HTTP)

Port 80 was identified as an active web service. Web services should be configured securely and should preferably use HTTPS for encrypted communication.

#### Port 135 (MSRPC)

MSRPC services are essential for Windows operations but may become attractive targets for attackers if not properly secured.

#### Port 445 (SMB)

SMB services facilitate file and printer sharing. However, SMB has historically been targeted by malware and ransomware attacks. Proper access control and patch management are required.

#### SQL Server Ports

SQL Server-related ports indicate active database services. Database servers should be protected using strong authentication and restricted network access.

---

## Wireshark Traffic Analysis

Network traffic analysis revealed the presence of several protocols.

### Protocols Observed

* TCP
* DNS
* HTTP
* HTTPS
* TLS
* ARP

### TCP Analysis

TCP packets established reliable communication sessions between devices. Most web-related traffic utilized TCP connections.

### DNS Analysis

DNS packets were generated whenever websites were accessed. DNS plays a critical role in resolving domain names into IP addresses.

### HTTP and HTTPS Analysis

Web browsing activities generated HTTP and HTTPS packets. HTTPS traffic was encrypted, thereby improving confidentiality and protecting transmitted information.

### TLS Analysis

TLS sessions were observed during secure communications. TLS ensures encryption, integrity, and confidentiality of network traffic.

---

## Security Risks Identified

The following potential risks were identified during the assessment.

### High Risk

#### Exposed SMB Services

SMB services are frequently targeted by attackers. Misconfigured SMB services can lead to unauthorized access and malware propagation.

#### Outdated Software

Unpatched services may contain known vulnerabilities that can be exploited by attackers.

---

### Medium Risk

#### Unnecessary Open Ports

Unused open ports increase the attack surface of the system.

#### Lack of Continuous Monitoring

Absence of network monitoring may delay the detection of suspicious activities.

---

### Low Risk

#### Routine Network Traffic

Normal web browsing traffic was observed and no suspicious communication patterns were identified during the assessment period.

---

## Risk Assessment Matrix

| Security Issue         | Risk Level |
| ---------------------- | ---------- |
| Exposed SMB Services   | High       |
| Outdated Services      | High       |
| Unnecessary Open Ports | Medium     |
| Lack of Monitoring     | Medium     |
| Normal Traffic         | Low        |

---

## Security Recommendations

To improve the security posture of the system, the following recommendations are suggested:

1. Regularly update the operating system and installed software.
2. Disable unnecessary services and close unused ports.
3. Restrict SMB access using firewall rules.
4. Enable strong authentication mechanisms.
5. Use HTTPS for all web services.
6. Continuously monitor network traffic.
7. Deploy firewalls and intrusion detection systems.
8. Perform periodic vulnerability assessments.
9. Conduct regular security audits.
10. Maintain proper backup and recovery procedures.

---

## Key Findings

* The local machine was active and reachable.
* Multiple services were running on the system.
* Open ports increased the system's attack surface.
* Encrypted HTTPS communication was observed.
* No suspicious traffic was detected during packet analysis.
* Several services require continuous monitoring and maintenance.

---

## Learning Outcomes

Through this assessment, the following skills and concepts were acquired:

* Network reconnaissance using Nmap.
* Service identification and enumeration.
* Packet capture using Wireshark.
* Protocol analysis and traffic inspection.
* Security risk identification.
* Preparation of professional security assessment reports.
* Understanding the importance of continuous monitoring.

---

## Conclusion

The network security assessment successfully evaluated the security posture of the local environment. Open ports, active services, and network communication patterns were identified and analyzed.

Although no critical malicious activity was observed, the assessment highlighted several areas that require continuous monitoring and security hardening.

Regular security assessments, timely software updates, strong access controls, and proactive monitoring are essential for maintaining a secure network environment and minimizing cybersecurity risks.

