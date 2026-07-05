# Task 4 - Internal Network Security Assessment

## Objective

Perform internal network enumeration and vulnerability assessment using Nmap to identify active hosts, open ports, running services, and recommend security improvements.

---

## Tools Used

- Nmap 7.99
- Windows 11
- Command Prompt

---

## Host Discovery

Command:

```bash
nmap -sn 192.168.0.0/24
```

### Active Hosts Found

| IP Address | Description |
|------------|-------------|
| 192.168.0.1 | TP-Link Router |
| 192.168.0.102 | Active Device |
| 192.168.0.114 | My Windows Laptop |
| 192.168.0.115 | Active Device |
| 192.168.0.116 | Active Device |

---

## Service Version Detection

Command:

```bash
nmap -sV 192.168.0.114
```

### Open Ports

| Port | Service | State |
|------|---------|-------|
| 135 | MSRPC | Open |
| 139 | NetBIOS | Open |
| 445 | Microsoft-DS (SMB) | Open |
| 5357 | Microsoft HTTPAPI | Open |

---

## Advanced Scan

Command:

```bash
nmap -A 192.168.0.114
```

### Findings

- Operating System: Microsoft Windows 11 (24H2–25H2)
- Device Type: General Purpose
- Network Distance: 0 Hops
- SMB Message Signing: Enabled and Required
- No critical vulnerabilities detected using default Nmap scripts.

---

## Security Recommendations

- Keep Windows updated.
- Enable Windows Defender Firewall.
- Disable unused services if not required.
- Restrict SMB access to trusted networks only.
- Perform regular vulnerability assessments.

---

## Screenshots

The following screenshots are included in this repository:

- packet_capture.png
- protocol_hierarchy.png
- endpoints_ipv4.png
- endpoints_ipv6.png
- conversations_ipv4.png
- conversations_ipv6.png
- host_discovery_scan.png
- service_version_scan.png
- advanced_scan.png

---

## Conclusion

The internal network assessment successfully identified active devices, detected open ports and running services, and confirmed that the system is using recommended SMB security settings. No critical vulnerabilities were identified during the assessment.
