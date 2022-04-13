# Eavesdrop

Author: [Rakhul KS](https://github.com/dedsec636)

Brief Description
![challenge picture](/static/challenge.png)

## Requirements

- Packet analysis using wireshark.
- Wireshark

## Source

 - [pcap file](/assets/capture.flag.pcap)

## Exploitation
 Analyzing the pcap file using strings shows us a chat conversation and also about a file transfer 
![strings output](/static/stringsoutput.png)

The openssl line shows us the password for the encrypted des3 data -supersecretpassword123

The conversation also mentions about transfer through port 9002 so now analyzing the pcap through wireshark,finding the 9002 port transfer we're able to see some data 
![wireshark](/static/wireshark.png)

Now exporting the packet bytes to a file named output.txt and then decrypting using openssl
![decrypt](/static/decryption.png)

We get the flag 
## Flag

picoCTF{nc_73115_411_91361db5}
