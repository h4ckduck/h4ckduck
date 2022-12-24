# Duckyscan Beta 1.2.3 #
Duckyscan is an advanced port analysis tool. It contains a set of tools, like nmap, whatweb... that are launched once the corresponding port is found open on the TARGET.
## Installation ##
Download the file and give it execute permission.
```
$ chmod u+x duckyscan
```
Then execute it
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
## Bugs ##
Duckyscan is still in Beta. Feel free to report bugs in Github (Issues).
