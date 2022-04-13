# Sleuthkit Apprentice

Author: [Rakhul KS](https://github.com/dedsec636)

Brief Description
![challenge picture](/forensics/sleuthkit%20apprentice/static/challenge.png)

## Requirements

- usage of autopsy 

## Source

- [disk img file](/forensics/sleuthkit%20apprentice/assets/disk.flag.img)

## Exploitation
Mounting the disk img on autopsy,we find mount 3 to have proper data
so doing a file name search of flag.txt results in a deleted file
![autopsy file seach picture](/forensics/sleuthkit%20apprentice/static/autopsyfilesearch.png)

Thus navigating to the directory where the deleted file is located results in 
a file flag.uni.txt while has the flag along with the unrecognized characters
![autopsy file](/forensics/sleuthkit%20apprentice/static/autopsy.png)

removing the unrecognized characters from the text results in the flag



## Flag

picoCTF{by73_5urf3r_152f373f}
