# Eavesdrop

Author: [Rakhul KS](https://github.com/dedsec636)

Brief Description
![challenge picture](/forensics/packets%20primer/static/challenge.png)

## Requirements

- Packet analysis using wireshark.
- Wireshark

## Source

- [pcap file](/forensics/packets%20primer/assets/network-dump.flag.pcap)

## Exploitation

 Analyzing the pcap file and following the first tcp stream results in the flag 

 (Also strings on the pcap file works)
 ![wireshark picture](/forensics/packets%20primer/static/wireshark.png)

Removing the spaces from the text results in the flag

## Flag

picoCTF{p4ck37_5h4rk_d0565941}
