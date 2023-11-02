
```bash
>>> nmap 192.168.1.0/24

Starting Nmap 7.94 ( https://nmap.org ) at 2023-11-02 11:57 India Standard Time
Nmap done: 256 IP addresses (0 hosts up) scanned in 207.53 seconds
```

<br>

```bash
>>> nmap -sT -vv -sC -p 8080 192.168.0.102

Starting Nmap 7.94 ( https://nmap.org ) at 2023-11-02 12:25 India Standard Time
NSE: Loaded 126 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 0.00s elapsed
NSE: Starting runlevel 2 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 0.00s elapsed
Initiating ARP Ping Scan at 12:25
Scanning 192.168.0.102 [1 port]
Completed ARP Ping Scan at 12:25, 0.23s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 12:25
Completed Parallel DNS resolution of 1 host. at 12:25, 5.54s elapsed
Initiating Connect Scan at 12:25
Scanning 192.168.0.102 [1 port]
Discovered open port 8080/tcp on 192.168.0.102
Completed Connect Scan at 12:25, 0.07s elapsed (1 total ports)
NSE: Script scanning 192.168.0.102.
NSE: Starting runlevel 1 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 5.08s elapsed
NSE: Starting runlevel 2 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 0.00s elapsed
Nmap scan report for 192.168.0.102
Host is up, received arp-response (0.14s latency).
Scanned at 2023-11-02 12:25:06 India Standard Time for 5s

PORT     STATE SERVICE    REASON
8080/tcp open  http-proxy syn-ack
| ssl-cert: Subject: commonName=IP Webcam
| Issuer: commonName=IP Webcam
| Public Key type: rsa
| Public Key bits: 2048
| Signature Algorithm: sha256WithRSAEncryption
| Not valid before: 2023-10-26T06:07:05
| Not valid after:  2030-10-25T06:07:05
| MD5:   8851:3db2:e90e:7c98:8d65:7bff:267f:8348
| SHA-1: 8f26:2577:72fc:34a5:6c4a:06ea:e970:7b9b:0b16:3efa
| -----BEGIN CERTIFICATE-----
| MIICpjCCAY6gAwIBAgIGAYtvvlOrMA0GCSqGSIb3DQEBCwUAMBQxEjAQBgNVBAMM
| CUlQIFdlYmNhbTAeFw0yMzEwMjYwNjA3MDVaFw0zMDEwMjUwNjA3MDVaMBQxEjAQ
| BgNVBAMMCUlQIFdlYmNhbTCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEB
| ALWlfaaBxT0bHO28XdcddVbEm5ufLqhtr+yt4mXCsObUIQcq0a16/FwlAFT3PV1x
| fhZrPZs4WPCSaojr7veVMmjT8ezTIYqRfgK/tyyVCiOBCR2yNuL5HAz6yHfyLv7Q
| Eqx1GD44WGSyht5SunWBGcn11B1FNtDuzXCL/si59fJ+GjuFnDx0GefZ0iKgmLRO
| d/oXsaI2YI6GeJnsrQlHCL8t/7CaqwOliCWzVonUp2bninuLCSX+XP661OT7y2/Q
| lnxIK2ZTpMXgoq89oQr8+1uF3kqFnn9/jx/9xlAmlOIyOyHZzka+bPRa8HR67XSB
| 8nUlwyXMlnYbS3FTbjt5Z90CAwEAATANBgkqhkiG9w0BAQsFAAOCAQEADWujjchW
| FKU8+8GQvfIyxdlW8ATCmtcSMTqCYR2Z6UcxodzVsHIBehUY06P5m0263iRyHCis
| LvwBeNjZE45455Kw+6F9O+IFg8Wl/g72NgxUVJJZ+aUMs4UwVEswe6Umw9ZM6Orm
| pUlgAWVR4JeTMIm4fMwjphHE5uxf176B3vJj4pke7N89bJThIkYS8w7Qotel7n2P
| vSDuNb390RlONVYKPi9LhJt5asByI7Mxef0XlSTJy88SA1Pe1bC4sJL9rGeeIfl0
| O04f5abPLjU59SoN2rO9ZVAO4sYNl4LrgNWDmgZKS8EPHHf3YfWIJnJ86hNK6yfy
| lODVjrb1lZkj/Q==
|_-----END CERTIFICATE-----
|_http-title: Site doesn't have a title.
| http-auth:
| HTTP/1.1 401 Unauthorized\x0D
|_  Digest qop=auth realm=IP Webcam nonce=1698908110
|_ssl-date: TLS randomness does not represent time
| http-methods:
|_  Supported Methods: GET HEAD POST OPTIONS
MAC Address: 1A:5C:85:C8:60:4A (Unknown)

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 0.00s elapsed
NSE: Starting runlevel 2 (of 2) scan.
Initiating NSE at 12:25
Completed NSE at 12:25, 0.00s elapsed
Read data files from: C:\Users\Vicky\Desktop\Repository\nmap\Nmap
Nmap done: 1 IP address (1 host up) scanned in 11.61 seconds
           Raw packets sent: 1 (28B) | Rcvd: 1 (28B)
```
