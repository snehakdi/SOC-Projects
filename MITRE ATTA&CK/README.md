#  MITRE ATT&CK – Wireshark Network Analysis 

###  Project Summary

This portfolio demonstrates the mapping of the Wireshark log analysis project MITRE ATTA&CK framework.

---

###  Tools & Environment

* Wireshark
* TCP/IP, TLS, QUIC, ARP, SSDP, IGMP
* MITRE ATT&CK Framework

---

###  Evidence (Screenshots)

* [Screenshot1](https://github.com/snehakdi/Security-Projects/blob/main/Wireshark-Analysis/Screenshots/screenshot1.png) – TCP, UDP, TLS overview
* [Screenshot2](https://github.com/snehakdi/Security-Projects/blob/main/Wireshark-Analysis/Screenshots/screenshot2.png) – TCP retransmission, ARP, SSDP
* [Screenshot3.png](https://github.com/snehakdi/Security-Projects/blob/main/Wireshark-Analysis/Screenshots/screenshot.png) – QUIC, IGMP, multicast traffic

---

### Observations & Analysis

#### Network Behaviors Identified

* TCP SYN attempts and retransmissions
* Encrypted TLSv1.2 and QUIC traffic over port 443
* ARP requests for local IP resolution
* SSDP M-SEARCH multicast traffic (239.255.255.250)
* IGMP  queries

---

### MITRE ATT&CK Mapping

| Observed Activity          | Tactic                   | Technique                              |
| -------------------------- | ------------------------ | -------------------------------------- |
| TCP connection attempts    | Discovery                | T1046 – Network Service Discovery      |
| ARP requests               | Discovery                | T1018 – Remote System Discovery        |
| SSDP M-SEARCH              | Discovery                | T1046 – Network Service Discovery      |
| TLS encrypted sessions     | Command & Control        | T1071 – Application Layer Protocol     |
| QUIC encrypted traffic     | Command & Control        | T1095 – Non-Application Layer Protocol |


> **Result:** No malicious intent detected

---


### Key Findings

* Traffic aligns with legitimate system behavior
* MITRE ATT&CK mapping enables clear communication



---

###  Conclusion

This project reflects **real workflows**—observe, analyze, map to MITRE, and report—using safe, real-world data from a clean environment.
