## Splunk Quick Cheat Sheet

**DNS Lookup**
```
| lookup dnslookup clientip as dest_ip OUTPUT clienthost as dest_host
```
**DNS Independent IP Resolution**
```
| inputlookup tHostInfo
| search src_ip=$IPADDRESS$ OR src_host=$HOSTNAME$
```

