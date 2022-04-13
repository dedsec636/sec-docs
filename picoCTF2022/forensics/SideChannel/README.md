# SideChannel

Author: [Rakhul KS](https://github.com/dedsec636)

Brief Description
![challenge picture](/static/challenge.png)

## Requirements

- understanding of timing based side channel attack

## Source

- [file](/assets/pin_checker)

## Exploitation
Reading about timing based side channel attacks lead me to bruteforce numbers initially and test out their response times using time 
Higher response times meant we were closer to the correct pin 
Random bruteforcing lead me to the pin 48390513 
## :P
![time picture](/static/bruteforcing.png)

using the pin we are able to get the flag

![final picture](/static/final.png)
## Flag

picoCTF{t1m1ng_4tt4ck_18704dda}

