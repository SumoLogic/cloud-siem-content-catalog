# [Mappings](README.md): Check Point Authorize Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Check Point|
|Product|Firewall|
|Log Format|JSON|
|Event ID Regex Pattern|`Authorize\|authorize`|

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
|ipProtocol|proto||
|srcDevice_ip|src||
|srcDevice_natIp|xlatesrc||
|timestamp|time|We expect the orginal record value of `time` is in the format `epoch`|

