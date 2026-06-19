# Network Traffic Investigation Lab

## Overview

This project demonstrates a basic network traffic investigation using Wireshark. The objective was to analyze a packet capture (PCAP) file, identify active hosts, investigate network conversations, review HTTP traffic, and document findings.


## Data Source

This investigation was conducted using a publicly available packet capture provided by Malware Traffic Analysis.

- Source: Malware Traffic Analysis
- Dataset: 2026-02-28 Traffic Analysis Exercise
- File: 2026-02-28-traffic-analysis-exercise.pcap

Reference:
https://www.malware-traffic-analysis.net/2026/02/28/2026-02-28-traffic-analysis-exercise.pcap.zip

The dataset was used solely for educational and research purposes as part of a network traffic investigation lab.


## Lab Environment

- Windows 11 Host
- Kali Linux VM
- Wireshark
- Public PCAP Sample

## Skills Demonstrated

- Packet Analysis
- Network Traffic Investigation
- Endpoint Analysis
- HTTP Traffic Analysis
- Incident Investigation
- Network Forensics
- Documentation and Reporting

---

## Investigation Process

### 1. Opened the PCAP file in Wireshark

Loaded the sample PCAP and reviewed overall capture statistics.

### 2. Reviewed Capture Properties

Collected information about:

- Packet count
- Capture duration
- Capture size
- Encapsulation type

### 3. Analyzed Endpoints

Used:

Statistics → Endpoints

to identify the most active hosts.

### 4. Analyzed Conversations

Used:

Statistics → Conversations

to identify communication patterns between systems.

### 5. Investigated HTTP Traffic

Applied:

http

filter to locate web traffic and identify requests and responses.

### 6. Documented Findings

Collected relevant indicators and summarized investigation results.

---

## Findings

- 15,512 packets captured
- Approximately 6.3 MB traffic analyzed
- Primary host identified: 10.2.28.88
- Multiple external communications observed
- Repeated HTTP POST requests detected
- Traffic directed toward external IP 45.131.214.85

---

## Indicators of Interest

| Type | Value |
|--------|---------|
| Internal IP | 10.2.28.88 |
| External IP | 45.131.214.85 |
| External IP | 4.149.160.182 |
| URI | /fakeurl.htm |
| Protocol | HTTP |

---

## Screenshots

### Capture Properties

![Capture Properties](Screenshots/Screenshot_01.png)

### Endpoint Analysis

![Endpoints](Screenshots/Screenshot_02.png)

### Conversation Analysis

![Conversations](Screenshots/Screenshot_03.png)

### HTTP Traffic Analysis

![HTTP Traffic](Screenshots/Screenshot_04.png)

---

## Conclusion

The investigation successfully identified active hosts, external communications, and web traffic activity within the packet capture. While no confirmed malicious activity was observed, the analysis demonstrates the workflow used by SOC analysts to investigate network traffic and identify indicators requiring further review.
