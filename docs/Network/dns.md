# A(Address) 和 CNAME(Canonical Name) 的差別
Canonical - 典範 ，可以理解為CNAME是用來給一個代號的

> The A record points a name to a specific IP.  
> The CNAME record points a name to another name, instead of an IP.  
> To summarize, an A record points a name to an IP. CNAME record can point a name to another CNAME or an A record.  

也就是說，A會指向IP，而CNAME是指向另一個name。

## 這有什麼用處?
CNAME可以當成子網域，指向A的地址
這樣如果A的IP有變，就只要改變A的對應就好，CNAME就不用動他。