# [Mappings](README.md): Zeek Weird Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Zeek|
|Product|Zeek|
|Log Format|JSON|
|Event ID Regex Pattern|`weird`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Bro|
|Product|Bro|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|name||
|device_ip|id.orig_h||
|dstDevice_ip|id.resp_h||
|dstPort|id.resp_p||
|srcPort|id.orig_p||
|timestamp|ts|We expect the orginal record value of `ts` is in the format `YYYY-MM-dd'T'HH:mm:ss.SSSSSSZ`|

