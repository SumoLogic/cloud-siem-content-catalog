# [Mappings](README.md): Fortinet Appctrl1

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|fortinet|
|Product|fortinet|
|Log Format|JSON|
|Event ID Regex Pattern|`webfilter`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Fortinet|
|Product|Fortigate|
|Record Type|NetworkProxy|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|----------------|-------------------|-----|
|action|action||
|application|app||
|bytesIn|rcvddelta||
|bytesOut|sentdelta||
|description|msg||
|device_hostname|devname||
|device_uniqueId|devid||
|dstDevice_ip|dstip||
|dstPort|dstport||
|http_hostname|hostname||
|ipProtocol|proto|This is a lookup field. More info to come in the catalog later...|
|normalizedSeverity|severity|This is a lookup field. More info to come in the catalog later...|
|packetsIn|rcvdpktdelta||
|packetsOut|sentpktdelta||
|sessionId|sessionid||
|severity|severity||
|srcDevice_ip|srcip||
|srcPort|srcport||
|timestamp|eventtime|We expect the original record value of `eventtime` is in the format `epoch`|
|user_username|user||

