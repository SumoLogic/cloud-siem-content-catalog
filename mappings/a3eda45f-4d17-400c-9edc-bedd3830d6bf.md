# [Mappings](README.md): McAfee Privilege Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|McAfee|
|Product|BeyondTrust Privilege Management|
|Log Format|CEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|McAfee|
|Product|BeyondTrust Privilege Management|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|description|cs3||
|device_ip|src||
|file_path|filePath||
|threat_name|cs6||
|timestamp|deviceCustomDate1|We expect the orginal record value of `deviceCustomDate1` is in the format `yyyy-MM-dd HH:mm:ss.S`|
|user_username|suser||

