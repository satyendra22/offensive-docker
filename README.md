<!-- markdownlint-disable MD033 MD041 -->

### Table of Contents

- [Links](#links)
- [Features](#features)
- [Requirements](#requirements)
- [Tools installed](#tools-installed)
  - [Operative system tools](#operative-system-tools)
  - [Network tools](#network-tools)
  - [Developer tools](#developer-tools)
  - [:hocho: Offensive tools](#hocho-offensive-tools)
    - [Port scanning](#port-scanning)
    - [:mag: Recon](#mag-recon)
      - [Subdomains](#subdomains)
      - [Subdomain takeover](#subdomain-takeover)
      - [DNS Lookups](#dns-lookups)
      - [:camera: Screenshot](#camera-screenshot)
      - [:spider_web: Crawler](#spider_web-crawler)
      - [:file_folder: Search directories](#file_folder-search-directories)
      - [Fuzzer](#fuzzer)
      - [Web Scanning](#web-scanning)
      - [CMS](#cms)
      - [Search JS](#search-js)
    - [Wordlist](#wordlist)
    - [Git repositories](#git-repositories)
    - [OWASP](#owasp)
    - [:iphone: Mobile](#iphone-mobile)
    - [Brute force](#brute-force)
    - [Cracking](#cracking)
    - [OS Enumeration](#os-enumeration)
    - [Exploits](#exploits)
    - [Windows](#windows)
    - [Reverse shell](#reverse-shell)
    - [Other resources](#other-resources)
  - [Forensic](#forensic)
  - [Custom functions](#custom-functions)
  - [Other services](#other-services)
  - [Reporting tools](#reporting-tools)
- [:memo: Documentation](#memo-documentation)
- [:hammer_and_wrench: Usage](#hammer_and_wrench-usage)
  - [Option 1 - Use the github repository](#option-1---use-the-github-repository)
  - [Option 2 - Use the image from docker hub](#option-2---use-the-image-from-docker-hub)
  - [Considerations to run the container](#considerations-to-run-the-container)
- [:gear: Nice configurations](#gear-nice-configurations)
  - [1. Configure credentials in the docker](#1-configure-credentials-in-the-docker)
  - [2. Alias to connect to HTB (Hack the Box) VPN](#2-alias-to-connect-to-htb-hack-the-box-vpn)
    - [Option 1 - HTB VPN using github repository](#option-1---htb-vpn-using-github-repository)
    - [Option 2 - HTB VPN using docker hub image](#option-2---htb-vpn-using-docker-hub-image)
  - [3. Save and load command history in your local environment](#3-save-and-load-command-history-in-your-local-environment)
    - [Option 1 - Command history using github repository](#option-1---command-history-using-github-repository)
    - [Option 2 - Command history using docker hub image](#option-2---command-history-using-docker-hub-image)
- [:white_check_mark: Environment tested](#white_check_mark-environment-tested)
- [:warning: Warning](#warning-warning)
- [:coffee: Donations](#coffee-donations)
- [Contributors](#contributors)
- [Contributing](#contributing)
- [:chart_with_upwards_trend: Stargazers over time](#chart_with_upwards_trend-stargazers-over-time)
- [License](#license)

## Links

- 🎬 Video: [Demos](https://asciinema.org/~aaaguirrep)
- 💬 Chat: [Discord](https://discord.gg/2uBfu8E)
- 🌟 [VPS Automation](https://github.com/aaaguirrep/offensive-docker-vps)
- 👉 [Advanced configurations](https://github.com/aaaguirrep/offensive-docker-custom)

## Features

- OS, networking, developing and pentesting tools installed.
- Connection to HTB (Hack the Box) vpn to access HTB machines.
- Popular wordlists installed: SecLists, dirb, dirbuster, fuzzdb, wfuzz and rockyou.
- Proxy service to send traffic from any browsers and burp suite installed in your local directory.
- Exploit database installed.
- Tool for cracking password.
- Linux enumeration tools installed.
- Tools installed to discovery services running.
- Tools installed to directory fuzzing.
- Monitor for linux processes without root permissions
- Zsh shell installed.

## Requirements

- Docker service installed

## Tools installed

### Operative system tools

- rdate
- vim
- zsh
- oh-my-zsh
- locate
- cifs-utils
- htop
- tree
- [gotop](https://github.com/cjbassi/gotop)
- fcrackzip

### Network tools

- traceroute
- telnet
- net-tools
- iputils-ping
- tcpdump
- openvpn
- whois
- host
- prips
- dig

### Developer tools

- git
- curl
- wget
- ruby
- go
- python
- python-pip
- python3
- python3-pip
- php
- aws-cli
- [tojson](https://github.com/tomnomnom/hacks/tree/master/tojson)
- nodejs

### :hocho: Offensive tools

#### Port scanning

- [nmap](https://github.com/nmap/nmap)
- [masscan](https://github.com/robertdavidgraham/masscan)
- [naabu](https://github.com/projectdiscovery/naabu)

#### :mag: Recon

##### Subdomains

- [Amass](https://github.com/OWASP/Amass)
- [GoBuster](https://github.com/OJ/gobuster)
- [Knock](https://github.com/guelfoweb/knock)
- [MassDNS](https://github.com/blechschmidt/massdns)
- [Altdns](https://github.com/infosec-au/altdns)
- [spyse](https://github.com/zeropwn/spyse.py)
- [Sublist3r](https://github.com/aboul3la/Sublist3r)
- [findomain](https://github.com/Edu4rdSHL/findomain)
- [subfinder](https://github.com/projectdiscovery/subfinder)
- [spiderfoot](https://github.com/smicallef/spiderfoot)
- [haktldextract](https://github.com/hakluke/haktldextract)

##### Subdomain takeover

- [subjack](https://github.com/haccer/subjack)
- [SubOver](https://github.com/Ice3man543/SubOver)
- [tko-subs](https://github.com/anshumanbh/tko-subs)

##### DNS Lookups

- [hakrevdns](https://github.com/hakluke/hakrevdns)

##### :camera: Screenshot

- [gowitness](https://github.com/sensepost/gowitness)
- [aquatone](https://github.com/michenriksen/aquatone)

##### :spider_web: Crawler

- [hakrawler](https://github.com/hakluke/hakrawler)
- [Photon](https://github.com/s0md3v/Photon)
- [gospider](https://github.com/jaeles-project/gospider)
- [gau](https://github.com/lc/gau)
- [otxurls](https://github.com/lc/otxurls)
- [waybackurls](https://github.com/tomnomnom/waybackurls)

##### :file_folder: Search directories

- [dirsearch](https://github.com/maurosoria/dirsearch)

##### Fuzzer

- [wfuzz](https://github.com/xmendez/wfuzz)
- [ffuf](https://github.com/ffuf/ffuf)

##### Web Scanning

- [whatweb](https://github.com/urbanadventurer/WhatWeb)
- [wafw00z](https://github.com/EnableSecurity/wafw00f)
- [nikto](https://github.com/sullo/nikto)
- [arjun](https://github.com/s0md3v/Arjun)
- [httprobe](https://github.com/tomnomnom/httprobe)
- [striker](https://github.com/s0md3v/Striker)
- [hakcheckurl](https://github.com/hakluke/hakcheckurl)
- [httpx](https://github.com/projectdiscovery/httpx)

##### CMS

- [wpscan](https://github.com/wpscanteam/wpscan)
- [joomscan](https://github.com/rezasp/joomscan)
- [droopescan](https://github.com/droope/droopescan)
- [cmseek](https://github.com/Tuhinshubhra/CMSeeK)

##### Search JS

- [LinkFinder](https://github.com/GerbenJavado/LinkFinder)
- [getJS](https://github.com/003random/getJS)
- [subjs](https://github.com/lc/subjs)

#### Wordlist

- [cewl](https://github.com/digininja/CeWL)
- wordlists:
  - [wfuzz](https://github.com/xmendez/wfuzz)
  - [SecList](https://github.com/danielmiessler/SecLists)
  - [Fuzzdb](https://github.com/fuzzdb-project/fuzzdb)
  - [Dirbuster](https://github.com/daviddias/node-dirbuster)
  - [Dirb](https://github.com/v0re/dirb)
  - [Rockyou](https://github.com/brannondorsey/naive-hashcat/releases/download/data/rockyou.txt)
  - [all.txt](https://gist.github.com/jhaddix/f64c97d0863a78454e44c2f7119c2a6a)
- crunch

#### Git repositories

- [gitleaks](https://github.com/zricethezav/gitleaks)
- [gitrob](https://github.com/michenriksen/gitrob)
- [gitGraber](https://github.com/hisxo/gitGraber)
- [github-search](https://github.com/gwen001/github-search)
- [GitTools](https://github.com/internetwache/GitTools)

#### OWASP

- [sqlmap](https://github.com/sqlmapproject/sqlmap)
- [XSStrike](https://github.com/s0md3v/XSStrike)
- [kxss](https://github.com/tomnomnom/hacks/tree/master/kxss)
- [dalfox](https://github.com/hahwul/dalfox)
- [jwt_tool](https://github.com/ticarpi/jwt_tool)
- [jaeles](https://github.com/jaeles-project/jaeles)

#### :iphone: Mobile

- [apktool](https://ibotpeaches.github.io/Apktool/)

#### Brute force

- [crowbar](https://github.com/galkan/crowbar)
- [hydra](https://github.com/vanhauser-thc/thc-hydra)
- [patator](https://github.com/lanjelot/patator)
- medusa

#### Cracking

- [hashid](https://github.com/psypanda/hashID)
- [john the ripper](https://github.com/magnumripper/JohnTheRipper)
- [hashcat](https://github.com/hashcat/hashcat)

#### OS Enumeration

- [htbenum](https://github.com/SolomonSklash/htbenum)
- [linux-smart-enumeration](https://github.com/diego-treitos/linux-smart-enumeration)
- [linenum](https://github.com/rebootuser/LinEnum)
- [enum4linux](https://github.com/portcullislabs/enum4linux)
- [ldapdomaindump](https://github.com/dirkjanm/ldapdomaindump)
- [PEASS - Privilege Escalation Awesome Scripts SUITE](https://github.com/carlospolop/privilege-escalation-awesome-scripts-suite)
- [Windows Exploit Suggester - Next Generation](https://github.com/bitsadmin/wesng)
- [smbmap](https://github.com/ShawnDEvans/smbmap)
- [pspy - unprivileged Linux process snooping](https://github.com/DominicBreuker/pspy)
- smbclient
- ftp

#### Exploits

- [searchsploit](https://github.com/offensive-security/exploitdb)
- [Metasploit](https://github.com/rapid7/metasploit-framework)
- [MS17-010](https://github.com/worawit/MS17-010)
- [AutoBlue-MS17-010](https://github.com/3ndG4me/AutoBlue-MS17-010)
- [PrivExchange](https://github.com/dirkjanm/PrivExchange)

#### Windows

- [evil-winrm](https://github.com/Hackplayers/evil-winrm)
- [impacket](https://github.com/SecureAuthCorp/impacket)
- [CrackMapExec](https://github.com/byt3bl33d3r/CrackMapExec)
- [Nishang](https://github.com/samratashok/nishang)
- [Juicy Potato](https://github.com/ohpe/juicy-potato)
- [PowerSploit](https://github.com/PowerShellMafia/PowerSploit)
- [pass-the-hash](https://github.com/byt3bl33d3r/pth-toolkit)
- [mimikatz](https://github.com/gentilkiwi/mimikatz)
- gpp-decrypt
- Netcat executables
- Plink executables

#### Reverse shell

- [netcat](https://github.com/diegocr/netcat)
- [rlwrap](https://github.com/hanslub42/rlwrap)

#### Other resources

- [pentest-tools](https://github.com/gwen001/offensive-tools) from [@gwen001](https://github.com/gwen001)
- [qsreplace](https://github.com/tomnomnom/qsreplace) from [@tomnomnom](https://github.com/tomnomnom)

### Forensic

- [exiftool](https://github.com/exiftool/exiftool)
- [steghide](https://github.com/StefanoDeVuono/steghide)
- [binwalk](https://github.com/ReFirmLabs/binwalk)
- [foremost](https://github.com/DogFive/foremost)

### Custom functions

- NmapExtractPorts from [@s4vitar](https://github.com/s4vitar)

### Other services

- apache2
- squid
- ssh
- rsyslog

### Reporting tools

- Latex
