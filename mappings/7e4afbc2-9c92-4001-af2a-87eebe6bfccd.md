# [Mappings](README.md): CylancePROTECT Device

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cylance|
|Product|Protect|
|Log Format|JSON|
|Event ID Regex Pattern|`Device$`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cylance|
|Product|Protect|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|Event Name||
|device_hostname|Device Name||
|device_ip|IP Address||
|device_mac|MAC Address||
|device_osName|OS||
|device_uniqueId|Device ID||
|user_username|Logged On Users||

