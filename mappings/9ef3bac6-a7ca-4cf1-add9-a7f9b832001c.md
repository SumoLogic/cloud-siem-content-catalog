# [Mappings](README.md): Unifi - Process sudo - Superuser Do Command Execution

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Log Format|JSON|
|Event ID Regex Pattern|`sudo-cmd`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Record Type|EndpointProcess|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|baseImage|syslog_process||
|commandLine|command||
|description|message||
|device_hostname|syslog_hostname||
|normalizedAction|None|The static text `execute` is populated in this schema field.|
|pid|syslog_process_id||
|user_username|user||

