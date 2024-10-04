# [Mappings](README.md): Symantec Agent Behavior Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Symantec|
|Product|Endpoint Protection|
|Log Format|JSON|
|Event ID Regex Pattern|`Agent Behavior Logs`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|Action||
|device_hostname|HostName||
|device_ip|IP_Address||
|file_hash_md5|Caller_MD5||
|file_path|Called_Process_Name||
|file_size|File_Size||
|normalizedAction|Action|This is a lookup field. More info to come in the catalog later...|
|success|Action|This is a lookup field. More info to come in the catalog later...|
|timestamp|Begin_Time|We expect the orginal record value of `Begin_Time` is in the format `yyyy-MM-dd HH:mm:ss`|
|user_username|UserName||

