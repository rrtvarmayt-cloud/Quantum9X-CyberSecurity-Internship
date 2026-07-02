# Task 2 - Network Traffic Analysis for Suspicious Activities

## Objective

Analyze network traffic using Wireshark to identify protocols, monitor communication between hosts, and detect suspicious network activity.

---

## Tools Used

- Wireshark 4.6.6
- Windows 11
- Internet Connection

---

## Procedure

1. Installed Wireshark.
2. Selected the active Wi-Fi interface.
3. Started packet capture.
4. Generated normal network traffic by:
   - Browsing websites
   - Opening Google services
   - Performing DNS lookups
5. Stopped packet capture and saved the capture as `Task2_Network_Capture.pcapng`.
6. Analyzed:
   - Protocol Hierarchy
   - Endpoints
   - Conversations

---

## Analysis Summary

### Protocol Hierarchy

The captured traffic mainly consisted of:

- IPv6
- IPv4
- TCP
- UDP
- QUIC
- TLSv1.2
- DNS
- ICMPv6

Most encrypted web traffic was carried over QUIC and TLS.

---

### Endpoints

Traffic was observed between:

- Local system
- Router
- External Internet servers

No unknown or suspicious endpoints were identified.

---

### Conversations

The majority of conversations were between the local host and trusted Internet services.

No abnormal communication patterns or unauthorized hosts were observed.

---

## Result

The captured traffic represented normal web browsing activity.

No suspicious packets, malware communication, or unauthorized devices were detected during the analysis.

---

## Conclusion

This task demonstrated how Wireshark can be used to capture and analyze network traffic, identify protocols, monitor communications, and verify whether suspicious activity exists on a network.

---

## Files Included

- Task2_Network_Capture.pcapng
- PacketCapture.png
- ProtocolHierarchy.png
- Endpoints.png
- Conversations.png
