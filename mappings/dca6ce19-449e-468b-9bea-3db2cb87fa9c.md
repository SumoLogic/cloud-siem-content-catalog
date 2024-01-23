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
|-----------------------|-------------------|-----|
|action|action||
|bytesIn|rcvdbyte||
|bytesOut|sentbyte||
|description|msg||
|device_ip|srcip||
|dstDevice_ip|dstip||
|dstPort|dstport||
|http_hostname|hostname||
|ipProtocol|proto||
|severity|apprisk||
|srcDevice_ip|srcip||
|srcPort|srcport||
|timestamp|eventtime|We expect the orginal record value of `eventtime` is in the format `epoch`|
|user_username|user||

