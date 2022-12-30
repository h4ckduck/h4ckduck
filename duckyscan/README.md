# Duckyscan Beta 1.2.3 #
Duckyscan is an advanced port analysis tool. It contains a set of tools, like nmap, whatweb... that are launched once the corresponding port is found open on the TARGET.

## How does it work? ##
When you execute Duckyscan, it launches Nmap which scans the ports of the TARGET. After that, it searches for possible exploits associated with the application version of that port. Finally, if the parameter "-a" is included in the execution of Duckyscan, it launches other tools to certain open ports. For example, if port 25 (SMTP) was found to be open, try to enumerate a number of users using netcat. This "add-ons tools" are called modules, and we will add more in the new versions of Duckyscan. You can submit yours at the Issues tab.

The goal of Duckyscan it is to automate tasks that have always been very repetitive during pentesting. 
## Installation ##
Download the file:
```
curl https://raw.githubusercontent.com/h4ckduck/h4ckduck/main/duckyscan/duckyscan > duckyscan
```
Give it execute permission:
```
$ chmod u+x duckyscan
```
Then execute it:
```
$ ./duckyscan
```
## Usage ##
```
	DUCKYSCAN beta 1.2.3 ( h4ckduck )
	Usage: 	duckyscan [IP] [OPTIONS]
		duckyscan [OPTIONS]

	OPTIONS:
	  -x --> Install (or upgrade) the required packages 
	  -h --> Display this info
	  -a --> Scan ports with scripts
	  -p --> Scan the chosen port/s
	  -n --> Save the Nmap scan
	  -s --> Save the scan in scan.hduck

	EXAMPLES:
	  duckyscan -a 192.168.0.0 -s
	  duckyscan -x
	  duckyscan -p 22,80,445 192.168.0.0
``` 
## Tools ##
* Nmap
* Searchsploit
* WhatWeb
* SMBclient
* NetCat
* FTP
* Nslookup
* Dig
## Bugs ##
Duckyscan is still in Beta. Feel free to report bugs in Github (Issues).
Please assign them to @focab0r
