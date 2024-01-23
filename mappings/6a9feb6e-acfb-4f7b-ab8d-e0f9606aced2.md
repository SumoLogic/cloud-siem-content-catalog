# [Mappings](README.md): Check Point Redirect

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Check Point|
|Product|Firewall|
|Log Format|JSON|
|Event ID Regex Pattern|`Redirect\|redirect`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|CheckPoint|
|Product|Firewall and VPN|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|device_ip|origin||
|dstDevice_ip|dst||
|dstPort|service||
|ipProtocol|proto||
|srcDevice_ip|src||
|srcDevice_natIp|xlatesrc||
|srcPort|s_port||
|timestamp|time|We expect the orginal record value of `time` is in the format `epoch`|
|user_username|user||

