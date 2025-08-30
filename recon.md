# Recon for Web Application

[**Main Link**](https://arenauser.notion.site/Recon-for-Web-Application-bc489086047f4320802b919f0cdeb70e)
- Initial Recon
    
    [**Censys**](https://search.censys.io/)
    
    [**Shodan**](https://www.shodan.io/)
    
    [**dnsdumpster**](https://dnsdumpster.com/)
    
    [**whois**](https://www.whois.com/)
    
    [**ViewDns**](https://viewdns.info/)
    
- Technology Discovery
    
    [Wappalyzer](https://www.wappalyzer.com/apps/)
    
    [BuiltWith](https://builtwith.com/toolbar)
    
    [WhatWeb](https://github.com/urbanadventurer/whatweb)
    
- Subdomain Discovery
    - Passive Sub Discovery
        - [**subfinder**](https://github.com/projectdiscovery/subfinder)
            - **Api Config file example (provider-config.yaml)**
         ```
         subfinder -v -d vulnweb.com | tee -a vulnweb-subfinder-in.txt
         ```
         
                File location will be `/root/.config/subfinder/provider-config.yaml` or `/home/.config/subfinder/provider-config.yaml`
                
                ```yaml
                bevigil: [WMoSVFE46rZhfTyG]
                binaryedge: [1fe5714c-931a-4207-bf8f-jfyronfi470]
                bufferover: [zxyj54ANcI5HcV69TRzdF43V1idade45sd4]
                builtwith: [af585278-7c1a-4982-8902-71a15e12d1f6]
                c99: []
                censys: [b9de5c68-5104:lf1C9nlaSRcjLQ9]
                certspotter: [k52506_aQNiXbl72wV9tbb3g]
                chaos: [7598c723-6b2b-4352-8e91-9789f7]
                chinaz: []
                dnsdb: []
                dnsrepo: []
                facebook: []
                fofa: []
                fullhunt: [e49e731a-c59d-4dc4-b299-702y]
                github: [ghp_UzZecHcIARVdDKY9rv6tuN6xLK]
                hunter: []
                intelx: [2.intelx.io:4844948d-6daf-430e]
                leakix: []
                netlas: []
                passivetotal: []
                quake: []
                redhuntlabs: [[https://reconapi.redhuntlabs.com/community/v1/domains/subdomains:vK68KXwi4Fsl514OVmve8gv](https://reconapi.redhuntlabs.com/community/v1/domains/subdomains:vK68KXwi4Fsl514OVmve8gvltlFVegCP)]
                robtex: []
                securitytrails: [utmpUb_5jh8oY0pX87Cf]
                shodan: [BP4MMEmxhkKlJwT7RfH3CUaMOOAY]
                threatbook: []
                virustotal: [f2097db4444f00efd12eed428f6444]
                whoisxmlapi: [at_JB0pXHzR8zzFbfS6MVPBcdmcmD]
                zoomeyeapi: [F3808CF8-b35F-F6093-54f3-492ec]
                ```

  
            - **Api Setup Guid**
                - **bevigil**
                    
                    **Note:** You can scan 50 times per month with this web application api. You can create another account to get another 50 cradit.😁
                    
                    [**Signup](https://bevigil.com/login)  (Enter any Email then put verification code to sign-up)**
                    
                    [**Api**](https://bevigil.com/osint/api-keys)
                    
                - **binaryedge**
                    
                    [**Sign-up**](https://app.binaryedge.io/sign-up)
                    
                    [**Api**](https://app.binaryedge.io/account/api)
                    
                    Put any name on the box to generate api.
                    
                - **bufferover**
                    
                    [Request a x-api-key](https://tls.bufferover.run/) (Submit email on free package 100 scan per month)
                    
                    You will get api through your email.
                    
                - **certspotter**
                    
                    [**Sign-up**](https://sslmate.com/signup?for=certspotter)
                    
                    [**Api**](https://sslmate.com/account/api_keys)
                    
                    Put any name and select Full Access. Then submit to get api key
                    
                - **chaos**
                    
                    [**Signup**](https://cloud.projectdiscovery.io/)
                    
                    [**Api**](https://cloud.projectdiscovery.io/scans?ref=api_key)
                    
                - **fullhunt**
                    
                    [**Sign-up**](https://fullhunt.io/signup/)
                    
                    [**Api**](https://fullhunt.io/user/settings/)
                    
                - **github**
                    
                    [**Sign-up**](https://github.com/signup)
                    
                    - Go to https://github.com/settings/tokens.
                    - Click on "Generate new token."
                    - Give your token a descriptive name (e.g.: "Subfinder").
                    - Select All repository.
                    - Click "Generate token."
                    - **Copy the generated token immediately. You won't be able to see it again.**
                - **intelx**
                    
                    [**Signup**](https://intelx.io/signup)
                    
                    [**Api**](https://intelx.io/account?tab=developer)
                    
                    **Api config formate:** [2.intelx.io:**API_key**]
                    
                - **redhuntlabs**
                    
                    [**Sign-up**](https://devportal.redhuntlabs.com/)
                    
                    [**Subscribe FREE**](https://devportal.redhuntlabs.com/)
                    
                    [**Api**](https://devportal.redhuntlabs.com/keys)
                    
                    **Api config formate:** [https://reconapi.redhuntlabs.com/community/v1/domains/subdomains:**API_Key**]
                    
                - **securitytrails**
                    
                    **Note: 50 Cradit free per month**
                    
                    [**Sign-up**](https://securitytrails.com/app/signup)
                    
                    [**Api**](https://securitytrails.com/app/account/credentials)
                    
                - **shodan**
                    
                    [**Register**](https://account.shodan.io/register)
                    
                    [**Api**](https://account.shodan.io/)
                    
                - **virustotal**
                    
                    [**Sign-up**](https://www.virustotal.com/gui/join-us)
                    
                    Api [[https://www.virustotal.com/gui/user/**Your_Username**/apikey]](https://www.virustotal.com/gui/user/Your_Username/apikey)
                    
                - **whoisxmlapi**
                    
                    **Note: 50 scan for trail trail**
                    
                    [**Sign-up**](https://main.whoisxmlapi.com/signup?lang=en)
                    
                    [**Api**](https://user.whoisxmlapi.com/products)
                    
                - **zoomeyeapi**
                    
                    [**Sign-up**](https://sso.telnet404.com/accounts/register/)
                    
                    [**Api**](https://www.zoomeye.org/profile)
                    
                - **builtwith**
                    
                    **Note: Dont use tempmail**
                    
                    [**Sign-up**](https://builtwith.com/signup)
                    
                    [**Api**](https://api.builtwith.com/)
                    
                
                **censys**
                
                netlas
                
                leakix
                
                passivetotal
                
                quake
                
                c99
                
                chinaz
                
                dnsdb
                
                dnsrepo
                
                fofa
                
                facebook
                
                threatbook
                
                robtex
                
                hunter
                
    - Active Sub Discovery
        - [Amass](https://github.com/owasp-amass/amass)
          ```
            amass enum -d vulnweb.com -active -v | tee -a vuln-active-sub.txt
          ```
        - [Puredns](https://github.com/d3mondev/puredns)
            
            ```
            git clone https://github.com/blechschmidt/massdns.git
            
            cd massdns
            
            make
            
            sudo make install
            
            go install github.com/d3mondev/puredns/v2@latest
            
            mkdir ~/.config/puredns
            
            nano ~/.config/puredns/resolvers.txt

            cat wordlist.text | puredns bruteforce vulnweb.com
            ```
            
- URL Discovery
    
    [**katana**](https://github.com/projectdiscovery/katana)

  ```
  katana -v -u vulnwev.com > vweb-urls.txt
  ```
    
    [**hakrawler**](https://github.com/hakluke/hakrawler)
    
    [**gau**](https://github.com/lc/gau)
    
    [**waybackurls**](https://github.com/tomnomnom/waybackurls)
  ```
  cat domains.txt | waybackurls > urls
  cat urls | httpx > active-urls.txt
  ```
    
- Parameter Discovery
    
    [**Paramspider**](https://github.com/devanshbatham/ParamSpider)

  ```
  apt install pipx
  pipx install git+https://github.com/devanshbatham/ParamSpider.git

  paramspider -d vulnwev.com > vwev-params.txt
  ```
    
    - **Gf-Patterns**
    
    ```bash
    #Installation_Command
    go install github.com/tomnomnom/waybackurls@latest
    
    #Pattern_Setup
    rm -rf /root/.gf && git clone https://github.com/1ndianl33t/Gf-Patterns /root/.gf
    
    #Example_Usage
    cat url.txt | gf sqli | tee -a sqli.txt
    ```
    
- Verify Active Items
    
    [**httpx**](https://github.com/projectdiscovery/httpx)
  ```
  cat wordlist.txt | httpx | tee -a vweb-httpx-active.txt
  httpx -l vwev-urls.txt
  httpx -l vwev-urls.txt -sc
  ```
    
    [**httprobe**](https://github.com/tomnomnom/httprobe)
    
- Visualization
    
    [**Aquatone**](https://github.com/michenriksen/aquatone)
    
- JavaScript
    
    [JSSCanner](https://github.com/dark-warlord14/JSScanner)
    [Secretfinder](https://github.com/m4ll0k/SecretFinder)
    
- File and Directory Discovery
    
    [Fuff](https://github.com/ffuf/ffuf) 
    [dirsearch](https://github.com/maurosoria/dirsearch)
    [wfuzz](https://github.com/xmendez/wfuzz)
    
- Wordlists
    
    [**Seclists**](https://github.com/danielmiessler/SecLists)
    
    [**PayloadBox**](https://github.com/payloadbox)
    
- Web Proxy
    
    Burp Suite Professional
    
    Owasp ZAP
    
- Scanners
    
    **Acunetix**
    
    **Nessus**
    
    **OpenVAS**
    
    [**Nmap**](https://github.com/nmap/nmap)
    
    [**Nikto**](https://github.com/sullo/nikto)
    
    [**Nuclei**](https://github.com/projectdiscovery/nuclei)
    
    [**SQLMap**](https://github.com/sqlmapproject/sqlmap)
    
    [**Ghauri**](https://github.com/r0oth3x49/ghauri)
    
    [**Dalfox**](https://github.com/hahwul/dalfox)
