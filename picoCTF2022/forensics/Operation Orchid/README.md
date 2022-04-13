# Operation Orchid

Author: [Rakhul KS](https://github.com/dedsec636)

Brief Description
![challenge picture](/forensics/Operation%20Orchid/static/challenge.png)

## Requirements

- autopsy usage

## Source

- [disk img](/forensics/Operation%20Orchid/assets/disk.flag.img.gz)

## Exploitation

 Analyzing the disk file in autopsy
 doing flag.txt file search in mount /3/ results in 

![autopsy search](/forensics/Operation%20Orchid/static/autopsysearch.png)

The flag.txt.enc results in salted hash 

going to the directory where the file is located leads to 

![directory search](/forensics/Operation%20Orchid/static/openssl.png)
the .ash_history file contains the openssl password for aes256

Thus decrypting using the openssl password leads to the flag 
![decrypt](/forensics/Operation%20Orchid/static/decrypt.png)

## Flag

picoCTF{h4un71ng_p457_cc87abb6}
