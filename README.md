## Splunk Quick Cheat Sheet

**Find out which HF receiving syslog**
```
 index=_* series IN (paloalto* fortinet*) host!=*splunkcloud*

| bin _time span=30m

| timechart values(series) by host
```
**DNS Independent IP Resolution**
```

```

