# [Mappings](README.md): AWS Redshift - Connection Log

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|AWS|
|Product|Redshift|
|Log Format|JSON|
|Event ID Regex Pattern|`(?i)(initiating\|disconnecting) session`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Amazon AWS|
|Product|Redshift|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|application|application_name||
|description|event_name||
|device_hostname|remote_host||
|device_osName|os_version||
|pid|pid||
|resource|database_name||
|sessionId|session_id||
|srcPort|remote_port||
|user_username|user_name||

