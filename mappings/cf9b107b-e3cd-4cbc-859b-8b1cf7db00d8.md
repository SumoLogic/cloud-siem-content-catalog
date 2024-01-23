# [Mappings](README.md): Linux OS Syslog - Process su - Switch User Failed

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Linux|
|Product|Syslog|
|Log Format|JSON|
|Event ID Regex Pattern|`su-failed`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Linux|
|Product|Linux OS Syslog|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|baseImage|syslog_process||
|changeTarget|user||
|device_hostname|syslog_hostname||
|pid|syslog_process_id||
|success|None|The static text `false` is populated in this schema field.|
|targetUser_username|user||
|user_userId|uid||
|user_username|ruser||

