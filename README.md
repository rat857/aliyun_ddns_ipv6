# 阿里云DDNS 转自"https://github.com/timwai/aliyunDDNS" 太好用了，怕被删，留个备份
* 为go设置代理
```shell
export GO111MODULE=on
export GOPROXY=https://goproxy.io
source /etc/profile
git clone https://ghproxy.com/https://github.com/rat857/aliyun_ddns_ipv6.git
go build
```

* 支持IPV4/IPV6
* 当type=AAAA时为IPV6，其它则为IPV4

```shell
./aliyunDDNS -domain mydomain.com -RR www -type AAAA -id 阿里云AccessKeyId -secret 阿里云AccessKeySecret
```
