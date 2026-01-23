# [Mappings](README.md): Unifi Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|msg||
|device_hostname|syslog_hostname||
|device_uniqueId|device_id||
|dstDevice_ip|dst_ip||
|pid|process_id||

