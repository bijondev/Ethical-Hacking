man nmap

nmap --help

nmap 192.168.1.1

nmap -sV 192.168.1.1

nmap --script vuln 192.168.1.4

nmap --script http-stored-xss 192.168.1.1

nmap -sn 192.168.66.0/24

nmap -sn 192.168.11.0/24

nmap -sL 192.168.0.1/24


What is the last IP address that will be scanned when your scan target is 192.168.0.1/27?

namp -sL 192.168.0.1/27

How many TCP ports are open on the target system at 10.10.39.40?

sudo nmap -sS -p- 10.10.39.40

What is the name and detected version of the web server running on 10.10.39.40?

nmap -sS -sV 10.10.39.40

nmap 192.168.139.1/24 -v

nmap -sS 192.168.139.1 -oA gateway

nman —sV -sC -D RND: 10 192 1680.106

nmap -SV -sC -D RND: 10 --spoof-mac dell 192168.0.106

nmap -SV -sC -D RND: 10 --spoof-mac dell 192168.0.106 -pN







Here are the Nmap flags with examples:

	1.	-sS (TCP SYN Scan)
 
Scans using SYN packets to determine open ports in a stealthy way.
Example:
```
nmap -sS 192.168.1.1
```

	2.	-sT (TCP Connect Scan)
Establishes a full TCP connection to determine open ports.
Example:
```
nmap -sT 192.168.1.1
```

	3.	-sU (UDP Scan)
Scans for open UDP ports.
Example:
```
nmap -sU 192.168.1.1
```

	4.	-p (Port specification)
Specify which ports to scan.
Example:
```
nmap -p 22,80,443 192.168.1.1
```

	5.	-sV (Service Version Detection)
Detects versions of services running on open ports.
Example:
```
nmap -sV 192.168.1.1
```

	6.	-O (OS Detection)
Attempts to detect the operating system of the target.
Example:

```
nmap -O 192.168.1.1
```

	7.	-A (Aggressive Scan)
Performs a comprehensive scan with OS detection, version detection, script scanning, and traceroute.
Example:
```
nmap -A 192.168.1.1
```

	8.	-T (Timing Template)
Sets scan speed/timing.
Example:
```
nmap -T4 192.168.1.1
```

	9.	-v (Verbose Output)
Increases output verbosity.
Example:
```
nmap -v 192.168.1.1
```

	10.	-n (Disable DNS resolution)
Skips DNS resolution for faster scans.
Example:
```
nmap -n 192.168.1.1
```

	11.	-PN (Treat all hosts as online)
Skips host discovery; assumes all hosts are online.
Example:
```
nmap -PN 192.168.1.1
```

	12.	-F (Fast Scan)
Scans fewer ports for quicker results.
Example:
```
nmap -F 192.168.1.1
```

	13.	-iL (Input from file)
Takes a list of targets from a file.
Example:
```
nmap -iL targets.txt
```

	14.	-oN (Normal Output)
Saves output in a human-readable format.
Example:
```
nmap -oN output.txt 192.168.1.1
```

	15.	-oX (XML Output)
Saves output in XML format.
Example:
```
nmap -oX output.xml 192.168.1.1
```

	16.	-oG (Grepable Output)
Generates output that is easy to parse with grep.
Example:
```
nmap -oG output.gnmap 192.168.1.1
```

	17.	--script (Run a Script)
Runs a specific script during the scan.
Example:
```
nmap --script=http-vuln-cve2017-5638.nse 192.168.1.1
```

	18.	-p- (Scan All Ports)
Scans all 65,535 TCP/UDP ports.
Example:
```
nmap -p- 192.168.1.1
```

	19.	-6 (IPv6 Scan)
Scans using IPv6.
Example:
```
nmap -6 2001:0db8::1
```

	20.	--open (Show only open ports)
Displays only open ports in the results.
Example:
```
nmap --open 192.168.1.1
```

	21.	--reason (Show reasons for port state)
Explains why a port is open/closed/filtered.
Example:
```
nmap --reason 192.168.1.1
```

	22.	--traceroute (Traceroute)
Performs a traceroute to the target.
Example:
```
nmap --traceroute 192.168.1.1
```

	23.	--script-args (Pass Arguments to Scripts)
Passes arguments to a script during the scan.
Example:
```
nmap --script=ssl-heartbleed --script-args=ssl-heartbleed.hostname=www.example.com 192.168.1.1
```

	24.	--max-retries (Max Retries)
Limits the number of retries if a port is not responding.
Example:
```
nmap --max-retries 2 192.168.1.1
```

	25.	--min-rate (Minimum Scan Rate)
Specifies the minimum number of packets to send per second.
Example:
```
nmap --min-rate 100 192.168.1.1
```

	26.	-p [port list] (Specific Ports)
Scan specific ports, such as 80, 443, and 8080.
Example:
```
nmap -p 80,443,8080 192.168.1.1
```

	27.	-R (DNS Resolution)
Resolves DNS names during the scan.
Example:
```
nmap -R 192.168.1.1
```

	28.	--version-all (Use all version detection probes)
Use all available probes for service version detection.
Example:
```
nmap --version-all 192.168.1.1
```

