<p align=center>
<img src="https://github.com/angelina-tsuboi/netspionage/blob/master/assets/banner.png" />
  <br />
  <br />
  <span>
  <b> Network Analysis CLI framework that performs Network Scanning, OSINT, and Attack Detection</b>
  </span>
  <br>
</p>

<p align="center">
  <a href="#installation">Installation</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#usage">Usage</a>
  &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#contributing">Contributing</a>
</p>

## Installation

```console
# clone the repo
git clone https://github.com/angelina-tsuboi/netspionage.git

# change the working directory to netspionage
cd netspionage

# install the requirements
pip3 install -r requirements.txt
```

## Usage

ReconSpider is very handy tool and easy to use. All you have to do is just have to pass values to parameter.
In order to start ReconSpider just type:
```
python3 netspionage.py
```

### Banner
```
                __             _                            
    ____  ___  / /__________  (_)___  ____  ____ _____ ____ 
   / __ \/ _ \/ __/ ___/ __ \/ / __ \/ __ \/ __ `/ __ `/ _ \
  / / / /  __/ /_(__  ) /_/ / / /_/ / / / / /_/ / /_/ /  __/
 /_/ /_/\___/\__/____/ .___/_/\____/_/ /_/\__,_/\__, /\___/ 
                    /_/                        /____/  
                    
 Created by Angelina Tsuboi [angelinatsuboi.net] V.0.0.1

 https://github.com/angelina-tsuboi/netspionage
 ----------------------------------------------------------------------------
 
 ENTER 1 - 4 TO SELECT OPTIONS

 1.  SCANNING                   Scan for IPs, nearby APs, ports, hosts, and more

 2.  RECONNAISSANCE             Gather  information  about nearby MAC addresses

 3.  DETECTION                  Detect for ARP Spoofing and SYN Flood attacks

 4.  EXIT                       Exit from netspionage to your terminal
 
```

**1. NETWORK SCANNER**

Gather information abuot devices connected to network such as IP address, MAC address, and OS.
```
netspionage >> 1
SCAN INPUT >> 1
NET IP ADDRESS (Eg: 192.168.1.1/24) >> 192.168.1.1/24
```

**2. WiFi SCANNER**

Gather information about nearby WiFi access points such as dBm Signal, SSID, channel, and encryption.
```
netspionage >> 1
SCAN INPUT >> 2
```

**3. PORT SCANNER**

Scan ports on a specified network to check if they are open or closed.
```
netspionage >> 1
SCAN INPUT >> 3
NET IP ADDRESS (Eg: 192.168.1.1/24) >> 192.168.1.1/24
```

**4. DNS MAP**

This option allows you to map an organizations attack surface with a virtual DNS Map of the DNS records associated with the target organization.
```
ReconSpider >> 4
DNS MAP (URL) >> vulnweb.com
```

**5. METADATA**

This option allows you to extract all metadat of the file.
```
Reconspider >> 5
Metadata (PATH) >> /root/Downloads/images.jpeg
```

**6. REVERSE IMAGE SEARCH**

This option allows you to obtain information and similar image that are available in internet.
```
Reconspider >> 6
REVERSE IMAGE SEARCH (PATH) >> /root/Downloads/images.jpeg
Open Search Result in web broser? (Y/N) : y
```

**7. HONEYPOT**

This option allows you to identify honeypots! The probability that an IP is a honeypot is captured in a "Honeyscore" value that can range from 0.0 to 1.0
```
ReconSpider >> 7
HONEYPOT (IP) >> 1.1.1.1
```

**8. MAC ADDRESS LOOKUP**

This option allows you to identify Mac address details who is manufacturer, address, country, etc.

```
Reconspider >> 8
MAC ADDRESS LOOKUP (Eg:08:00:69:02:01:FC) >>
```

**9. IPHEATMAP**

This option provided you heatmap of the provided ip or single ip, if connect all the provided ip location with accurate Coordinator.
```
Reconspider >> 9

    1) Trace single IP
    2) Trace multiple IPs
OPTIONS >>
```

**10. TORRENT**

This option allows you to gathers history of Torrent download history.
```
Reconspider >> 10
IPADDRESS (Eg:192.168.1.1) >>
```

**11. USERNAME**

This option allows you to gathers account information of the provided username from social media like Instagram, Twitter, Facebook.
```
Reconspider >> 11

1.Facebook
2.Twitter
3.Instagram

Username >>
```

**12. IP2PROXY**

This option allows you to identify whether IP address uses any kind of VPN / Proxy to hide his identify.
```
Reconspider >> 12
IPADDRESS (Eg:192.168.1.1) >>
```

**13. MAIL BREACH**

This option allows you to identify all breached mail ID from given domain.
```
Reconspider >> 13
DOMAIN (Eg:intercom.io) >>
```

**99. UPDATE**

This option allows you to check for updates. If a newer version will available, ReconSpider will download and merge the updates into the current directory without overwriting other files.
```
ReconSpider >> 99
Checking for updates..
```

**0. EXIT**

This option allows you to exit from ReconSpider Framework to your current Operating System's terminal.
```
ReconSpider >> 0
Bye, See ya again..
```

## Contributing
We would love to have you help us with the development of Sherlock. Each and every contribution is greatly valued!

Here are some things we would appreciate your help on:
- Addition of new site support ¹
- Bringing back site support of [sites that have been removed](removed_sites.md) in the past due to false positives

[1] Please look at the Wiki entry on [adding new sites](https://github.com/sherlock-project/sherlock/wiki/Adding-Sites-To-Sherlock)
to understand the issues.

TODO:
- test on VM with PAU06
- fix tcp flood attack

- make shortform command of netspionage
- write documentation
- upload to pypi

