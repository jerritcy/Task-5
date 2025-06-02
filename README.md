#  Task 5 - Wireshark Packet Analysis

## Objective
The goal of this task was to use Wireshark to capture live network packets, identify at least three different protocols, and analyze the traffic patterns. This task helps build practical skills in packet inspection, protocol awareness, and network troubleshooting.

---

## Tools Used
- **Wireshark** 
- **Active Network Interface** (Wi-Fi)

---

## Steps Performed

1. Installed Wireshark.
2. Started packet capture on the active interface.
3. Browsed websites like YouTube and Google to generate traffic.
4. Stopped capture after one minute.
5. Filtered packets using protocol filters: `snmp`, `dns`, `quic`, `tcp`.
6. Exported the capture as a `.pcap` file.
7. Documented key findings in this README.

---

## Protocols Identified

### 1. SNMP (UDP 161)
Used for network device monitoring. Observed a GET-NEXT request between two local IPs with community string "public".

### 2. DNS (UDP 53)
Resolves domain names. Captured queries to youtube.com, google.com, etc., with responses showing multiple A-records.

### 3. QUIC (UDP 443)
Encrypted transport protocol used in HTTP/3. Seen communicating with Google servers using handshake and encrypted payloads.

### 4. TCP (Various Ports)
Reliable transport protocol. Included TLS handshakes with Microsoft servers and some connections ending in reset (RST).

---

## Files Included
- Wireshark Analysis.pdf
  

---

## Key Concepts Demonstrated
- Packet capture and filtering
- Protocol analysis: SNMP, DNS, QUIC, TCP
- Network troubleshooting
- Understanding encrypted and unencrypted traffic

---
