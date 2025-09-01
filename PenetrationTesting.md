#tools

https://bgp.he.net/

[**mapCIDR**](https://github.com/projectdiscovery/mapcidr)

```
mapcidr -cidr 173.0.84.0/24
```


[**dnsx**](https://github.com/projectdiscovery/dnsx)

```
subfinder -silent -d hackerone.com | dnsx -silent

subfinder -silent -d hackerone.com | dnsx -silent -a -resp-only

subfinder -silent -d hackerone.com | dnsx -silent -cname -resp

subfinder -silent -d hackerone.com | dnsx -silent  -asn

subfinder -silent -d hackerone.com | dnsx -silent -rcode noerror,servfail,refused

echo 173.0.84.0/24 | dnsx -silent -resp-only -ptr

echo AS17012 | dnsx -silent -resp-only -ptr

dnsx -silent -d facebook.com -w dns_worldlist.txt

dnsx -silent -d domains.txt -w jira,grafana,jenkins

cat domains.txt | dnsx -silent -w jira,grafana,jenkins -d -

dnsx -d google.FUZZ -w tld.txt -resp

dnsx -l subdomain_list.txt -wd airbnb.com -o output.txt
```

[**aix**](https://github.com/projectdiscovery/aix)

[**pdtm**](https://github.com/projectdiscovery/pdtm)

[**naabu**](https://github.com/projectdiscovery/naabu)

```
naabu -host hackerone.com

naabu -p 80,443,21-23,u:53 -host hackerone.com

naabu -p - -exclude-ports 80,443

naabu -list hosts.txt

naabu -host 104.16.99.52 -json

echo hackerone.com | naabu -silent | httpx -silent

echo hackerone.com | dnsx -resp-only -a -aaaa -silent | naabu -p 80 -silent

echo hackerone.com | ./naabu -p 80 -ip-version 6

echo hackerone.com | ./naabu -iv 4,6 -sa -p 80 -silent

echo hackerone.com | naabu -nmap-cli 'nmap -sV -oX nmap-output'

```

[**RustScan**](https://github.com/bee-san/RustScan)


[**ASNmap**](https://github.com/projectdiscovery/asnmap)

```
echo GOOGLE | ./asnmap -silent

asnmap -a AS45596 -silent

asnmap -i 100.19.12.21 -silent

asnmap -d hackerone.com -silent

asnmap -org GOOGLE -silent

echo hackerone.com | ./asnmap -json -silent | jq

echo hackerone.com | ./asnmap -csv -silent


```

[**notify**](https://github.com/projectdiscovery/notify)

```
subfinder -d hackerone.com | notify -bulk

subfinder -d hackerone.com -o h1.txt; notify -data h1.txt

subfinder -d hackerone.com -o h1.txt; notify -data h1.txt -bulk -provider discord,slack

subfinder -d hackerone.com -o h1.txt; notify -data h1.txt -bulk -id recon,vulns,scan

subfinder -d intigriti.com | httpx | nuclei -tags exposure -o output.txt; notify -bulk -data output.txt

notify -provider-config providers.yaml


```

[**nuclei**](https://github.com/projectdiscovery/nuclei)

amass

[**oneForAll**] (https://github.com/shmilylty/OneForAll/blob/master/docs/en-us/README.md)

```
nuclei -target https://example.com

nuclei -list urls.txt

nuclei -target 192.168.1.0/24

nuclei -u https://example.com -t /path/to/your-template.yaml

nuclei -target https://example.com -dashboard


```

[**subdominator**]()

[**finddomain**](https://github.com/Findomain/Findomain)

# Technology Discovery
origin ip
server
programming language

# Asset Discovery

dir brute / peram fuzz / crawling

[**uff**](https://github.com/sw33tLie/uff)

```
echo hi | uff -c -u http://example.com -w - -opaque "http://127.0.0.1/FUZZ"

echo "hi" | uff -c -u http://example.com/FUZZ -w - -H '   I AM AN INVALID: HEADER'

echo hi | uff -c -u http://example.com/FUZZ -w - -H 'lowercase-header: yes'

echo "hi" | uff -u "http://1y0urh3t90pydzt4ws733i1gv71zppde.oastify.com/" -w - -X "GET /FUZZ HTTP/1.0
x: x"

echo "hi" | uff -u "http://pb4i45ghmo2mqn6s9gkrg6e48veo2eq3.oastify.com/" --method-as-raw-request -w -  -c  -X $'GET /FUZZ HTTP/0.9\r\nHost: {HOST}\r\n look im just a raw request lol \r\n   so raw\r\n\r\n'

echo hi | go run *.go -c -request /tmp/req.txt -u "http://7w40pn1z76n4b5rauy591ozmtdzan0bp.oastify.com" -w - -debug-log asd
```

[**dirsearch**](https://github.com/maurosoria/dirsearch)

```
python3 dirsearch.py -u https://target

python3 dirsearch.py -e php,html,js -u https://target

python3 dirsearch.py -e php,html,js -u https://target -w /path/to/wordlist

python3 dirsearch.py -e php,html,js -u https://target -r

python3 dirsearch.py -e php,html,js -u https://target -r --max-recursion-depth 3 --recursion-status 200-399

python3 dirsearch.py -e php,html,js -u https://target -r --exclude-subdirs image/,media/,css/

python3 dirsearch.py -e php,htm,js,bak,zip,tgz,txt -u https://target -t 20

python3 dirsearch.py -e php -u https://target --prefixes .,admin,_

python3 dirsearch.py -e php -u https://target --suffixes ~

python3 dirsearch.py -e php,html,js -u https://target --exclude-sizes 1B,243KB

python3 dirsearch.py -e php,html,js -u https://target --exclude-texts "403 Forbidden"

python3 dirsearch.py -e php,html,js -u https://target --exclude-regexps "^Error$"

python3 dirsearch.py -e php,html,js -u https://target --exclude-redirects "https://(.*).okta.com/*"

python3 dirsearch.py -e php,html,js -u https://target --exclude-response /error.html

python3 dirsearch.py -e php,html,js -u https://target --subdirs /,admin/,folder/

python3 dirsearch.py -e php,html,js -u https://target --proxy 127.0.0.1:8080

python3 dirsearch.py -e php,html,js -u https://target --proxy socks5://10.10.0.1:8080

python3 dirsearch.py -e php,html,js -u https://target --proxylist proxyservers.txt

python3 dirsearch.py -e php -l URLs.txt --format plain -o report.txt

python3 dirsearch.py -e php -u https://target --format html -o target.json

cat urls.txt | python3 dirsearch.py --stdin

python3 dirsearch.py -u https://target --max-time 360

python3 dirsearch.py -u https://target --auth admin:pass --auth-type basic

python3 dirsearch.py -u https://target --header-list rate-limit-bypasses.txt
```

[**x8**](https://github.com/Sh1Yo/x8)

```
x8 -u "https://example.com/" -w <wordlist>

x8 -u "https://example.com/?something=1" -w <wordlist>

x8 -u "https://example.com/" -X POST -w <wordlist>

x8 -u "https://example.com/" -X POST -b '{"x":{%s}}' -w <wordlist>

x8 -u "https://example.com/" -X POST -b '{"x":{%s}}' -w <wordlist>

x8 -u "https://example.com/" "https://4rt.one/" -W0

x8 -u "https://example.com/" --param-template "user[%k]=%v" -w <wordlist>

x8 -u "https://example.com/?path=..%2faction.php%3f%s%23" --encode -w <wordlist>

x8 -u "https://example.com" --headers -w <wordlist>

x8 -u "https://example.com" --headers -H "Cookie: %s" -w <wordlist>


```

[**arjun**](https://github.com/s0md3v/Arjun)

[**katana**](https://github.com/projectdiscovery/katana)

```
katana -u https://tesla.com

katana -u https://tesla.com,https://google.com

katana -list url_list.txt

echo https://tesla.com | katana

cat domains | httpx | katana

katana -u https://tesla.com -headless -no-sandbox

katana -u https://tesla.com -headless -no-incognito

katana -u https://tesla.com -headless -system-chrome -headless-options --disable-gpu,proxy-server=http://127.0.0.1:8080

katana -u https://tesla.com -fs dn

katana -u https://tesla.com -cs in_scope.txt

katana -u https://tesla.com -cos logout

katana -u https://tesla.com -cos out_of_scope.txt

katana -u https://tesla.com -do

katana -u https://tesla.com -d 5

katana -u https://tesla.com -jc

katana -u https://tesla.com -ct 2

katana -u https://tesla.com -kf robotstxt,sitemapxml

katana -u https://tesla.com -aff

katana -u https://tesla.com -H 'Cookie: usrsess=AmljNrESo'

katana -u https://tesla.com -H cookie.txt

katana -headless -u https://tesla.com -cwu ws://127.0.0.1:9222/devtools/browser/c5316c9c-19d6-42dc-847a-41d1aeebf7d6 -no-incognito

katana -u https://tesla.com -f qurl -silent

katana -u https://tesla.com -f email,phone

katana -u https://tesla.com -sf key,fqdn,qurl -silent

katana -u https://tesla.com -silent -em js,jsp,json

katana -u https://tesla.com -silent -ef css,txt,md

katana -u https://tesla.com -mr 'https://shop\.tesla\.com/*' -silent

katana -u https://tesla.com -fr 'https://www\.tesla\.com/*' -silent

katana -u https://www.hackerone.com -mdc 'status_code == 200'

katana -u https://www.hackerone.com -mdc 'contains(endpoint, "default") && status_code != 403'

katana -u https://www.hackerone.com -mdc 'contains(to_lower(technologies), "php")'

katana -u https://www.hackerone.com -fdc 'contains(to_lower(technologies), "cloudflare")'

katana -u https://www.hackerone.com -fdc 'contains(to_lower(technologies), "cloudflare")'

katana -u https://tesla.com -delay 20

katana -u https://tesla.com -p 20

katana -u https://tesla.com -rl 100

katana -u https://tesla.com -rlm 500

katana -u https://example.com -no-scope -output example_endpoints.txt

katana -u https://example.com -output-template '{{email}} - {{url}}'

katana -u https://example.com -jsonl | jq .

katana -u https://example.com -no-scope -store-response


```

[https://burpbounty.net/](https://burpbounty.net/releases/)
