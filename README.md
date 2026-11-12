Wireshark Traffic Analysis Lab
Objective:  Analyze live network traffic using Wireshark.

Tools Used:
    Ubuntu 26.04 LTS
    Wireshark 4.6.4
    Firefox

DNS Analysis
Findings:
    Source IP: 10.0.2.15
    DNS Server: 192.168.1.1
    Domain observed:
        detectorportal.firefox.com
        mozilla.map.fastly.net

Analysis:
The Ubuntu VM sent DNS requests to the DNS server. The DNS server responded with domain resolution information.

Lessons Learned:
- DNS converts domain names into IP addresses.
- Wireshark can capture and analyze live network traffic.
- DNS queries and responses can be observed in real time.



TLS Analysis
Filter Used: tls

Findings:
    Observed TLSv1.3 encrypted traffic.
    HTTPS communication was occurring over port 443.
    Traffic was exchanged between the Ubuntu VM and external servers.

Analysis:
TLSv1.3 was used to encrypt network communications. This prevents attackers from viewing the contents of transmitted data and helps protect user privacy and security.
