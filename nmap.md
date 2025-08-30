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
