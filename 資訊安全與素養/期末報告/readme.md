
##  期末報告:我的第一份網路鑑識實戰手技(network Forensics)
- Forensics
- wireshark
  - [download](https://www.wireshark.org/download.html)
  -  
- network forensic

#### 簡報內容
```
Forensics數位鑑識
網絡概論
Network forensics
Wireshark
CTF
```
#### 參考資料
- [數位鑑識](https://zh.wikipedia.org/wiki/%E6%95%B8%E4%BD%8D%E9%91%91%E8%AD%98)
- [網路鑑識](https://www.geeksforgeeks.org/what-is-network-forensics/)
- [網路鑑識](https://en.wikipedia.org/wiki/Network_forensics)


# computer network
- Network devices and Hareware
  - repeater
  - hub
  - bridge
  - switch
  - router
  - L3-switch
  - L4-switch
  - L7-switch
  - proxy
- OSI model, TCP/IP
  - OSI Model
  - TCP/IP
- TCP/IP protocal suites 
  - Application Layer
    - HTTP vs HTTPS 
  - Trasnport Layer
  - Interconnecting Layer 
- [Network Topology](https://en.wikipedia.org/wiki/Network_topology)
- Networking Commands
  - Windows Networking Commands
  - Linux Networking Commands


## HTTP
- HTTP Client vs Server
  - HTTP Clients: 
    - Python
- http request
  - [HTTP request methods HTTP 1.1八大方法](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)
  - [Request header](https://developer.mozilla.org/en-US/docs/Glossary/Request_header#:~:text=A%20request%20header%20is%20an,preferred%20formats%20of%20the%20response.)
- http Response
  - [狀態碼 status code](https://zh.wikipedia.org/zh-tw/HTTP%E7%8A%B6%E6%80%81%E7%A0%81#5xx%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%94%99%E8%AF%AF)
  - [Response header](https://developer.mozilla.org/en-US/docs/Glossary/Response_header) 

## a GET request:
```html
GET /home.html HTTP/1.1
Host: developer.mozilla.org
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10.9; rv:50.0) Gecko/20100101 Firefox/50.0
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8
Accept-Language: en-US,en;q=0.5
Accept-Encoding: gzip, deflate, br
Referer: https://developer.mozilla.org/testpage.html
Connection: keep-alive
Upgrade-Insecure-Requests: 1
If-Modified-Since: Mon, 18 Jul 2016 02:36:04 GMT
If-None-Match: "c561c68d0ba92bbeb8b0fff2a9199f722e3a621a"
Cache-Control: max-age=0
```
