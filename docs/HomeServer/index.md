## Model
* NanoPi R5S
* RAM: 4GB
* SSD: 1TB
* 

## Smartdns

## iperf3 內網測速

#### Server端
`iperf3 -s` : 臨時開啟
`iperf3 -s -D` : 開啟在後台常駐執行

#### Client端
`iperf3 -c 192.168.100.1 ` : 單線程測試，網址server所在位址  
`iperf3 -c 192.168.100.1 -b 1000m -t 30 -i 1 -u -P 2` : 2線程UDP測速, 測試30秒

## crontab寫法