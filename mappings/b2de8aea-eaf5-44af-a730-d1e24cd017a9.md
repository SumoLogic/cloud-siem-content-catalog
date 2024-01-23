# [Mappings](README.md): McAfee MVISION Endpoint

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|McAfee|
|Product|MVISION Endpoint|
|Log Format|CEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|McAfee|
|Product|Endpoint Security|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|description|Event Name||
|device_hostname|dhost||
|device_ip|src||
|device_natIp|src||
|file_path|filePath||
|severity|severity|This is a lookup field. More info to come in the catalog later...|
|timestamp|deviceCustomDate1|We expect the orginal record value of `deviceCustomDate1` is in the format `yyyy-MM-dd HH:mm:ss.SSS`|
|user_username|suser||

