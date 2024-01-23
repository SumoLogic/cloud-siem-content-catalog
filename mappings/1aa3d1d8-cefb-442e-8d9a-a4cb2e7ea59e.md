# [Mappings](README.md): McAfee Avecto Defendpoint

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|McAfee|
|Product|Avecto Defendpoint|
|Log Format|CEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|McAfee|
|Product|Avecto Defendpoint|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|commandLine|Content.CommandLine||
|description|Event Name||
|device_hostname|dhost||
|device_ip|src||
|device_mac|MachineInfo.RawMACAddress||
|device_natIp|src||
|device_osName|MachineInfo.OSName||
|file_basename|Content.Description||
|file_hash_md5|Content.MD5||
|file_path|filePath||
|parentBaseImage|Content.ParentProcessFileName||
|parentPid|parentPid||
|pid|Content.ProcessID||
|processUid|Content.UniqueProcessID||
|severity|severity|This is a lookup field. More info to come in the catalog later...|
|threat_name|Threat Name||
|timestamp|deviceCustomDate1|We expect the orginal record value of `deviceCustomDate1` is in the format `yyyy-MM-dd HH:mm:ss.SSS`|
|user_authDomain|Content.UserDomainName||
|user_userId|Content.UserSID||
|user_username|suser||

