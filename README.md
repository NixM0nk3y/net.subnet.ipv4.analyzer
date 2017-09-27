# net.subnet.ipv4.analyzer

### This script will parse your defined networks and subnets and print any undefined ip space.
example:
```
$ cat networks.txt 
127.0.0.0/22
```
```
$ cat subnets.txt 
127.0.0.0/30
127.0.0.64/29
127.0.1.0/25
```
```
$ ./free_subnets.py 
Available IP subnets
START:      127.0.0.32	END:      127.0.0.63	SIZE: 32 (/27)
START:      127.0.0.16	END:      127.0.0.31	SIZE: 16 (/28)
START:       127.0.0.8	END:      127.0.0.15	SIZE:  8 (/29)
START:       127.0.0.4	END:       127.0.0.7	SIZE:  4 (/30)
START:     127.0.0.128	END:     127.0.0.255	SIZE:128 (/25)
START:      127.0.0.96	END:     127.0.0.127	SIZE: 32 (/27)
START:      127.0.0.80	END:      127.0.0.95	SIZE: 16 (/28)
START:      127.0.0.72	END:      127.0.0.79	SIZE:  8 (/29)
START:       127.0.3.0	END:     127.0.3.255	SIZE:256 (/24)
START:       127.0.2.0	END:     127.0.2.255	SIZE:256 (/24)
START:     127.0.1.128	END:     127.0.1.255	SIZE:128 (/25)
```
