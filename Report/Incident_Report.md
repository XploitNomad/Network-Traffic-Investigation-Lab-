# Incident Investigation Report

## Summary

A packet capture file was analyzed using Wireshark to identify network activity, active systems, and web traffic patterns.

## Scope

- Endpoint Analysis
- Conversation Analysis
- HTTP Investigation

## Findings

### Active Internal Host

10.2.28.88

### External Communications

- 45.131.214.85
- 4.149.160.182
- 13.69.116.109

### HTTP Activity

Observed multiple HTTP POST requests to:

http://45.131.214.85/fakeurl.htm

### Traffic Statistics

- Packets: 15,512
- Duration: 4h 21m
- Size: 6.3 MB

## Assessment

No confirmed malicious activity identified.

Further investigation would be recommended in a production environment.


