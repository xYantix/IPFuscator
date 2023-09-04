# IPFuscator

## Author

Vincent Yiu (@vysecurity)
Python 3 support added by CJ (@xyantix)

## Blog Post
https://vincentyiu.co.uk/ipfuscation/

## What is IPFuscator?

IPFuscation is a technique that allows for IP addresses to be represented in hexadecimal or decimal instead of the decimal encoding we are used to. IPFuscator allows us to easily convert to these alternative formats that are interpreted in the same way.

## Usage

1) `git clone https://github.com/vysec/ipfuscator`
2) `python ipfuscator.py 127.0.0.1` or `python3 ipfuscator3.py 127.0.0.1` 

```
IPFuscator
Author: Vincent Yiu (@vysecurity)
https://www.github.com/vysec/IPFuscator
Version: 0.2.0

IP Address:     127.0.0.1

Decimal:        2130706433
Hexadecimal:    0x7f000001
Octal:          017700000001

Full Hex:       0x7f.0x0.0x0.0x1
Full Oct:       0177.0.0.01

Random Padding:
Hex:    0x000000000007f.0x000000000000000000000000000000.0x0000.0x0000000000000000000000001
Oct:    00000000000000000000000177.000000000000000000.00000000000000000000000000000.000001

Random base:
#1:     0x7f.0x0.0.01
#2:     0x7f.0x0.0x0.1
#3:     0177.0x0.0x0.0x1
#4:     0x7f.0.0.01
#5:     127.0x0.0.0x1

Random base with random padding:
#1:     127.0x00000000.000000.000000000000000001
#2:     127.0x0000000000000.0x00000000000000000000000000000.0001
#3:     0000000000000000177.0x0000000000000000000000.0x00000000000000000000000000.1
#4:     0000000000000000000177.0.000000.1
#5:     127.0000000000000000000000.0x0000000000000000000.000000000000000000000000000001
```

3) Take any representation and use it in commands such as `ping`. You can also use it for a command and control endpoint.
