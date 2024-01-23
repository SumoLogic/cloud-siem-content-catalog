# [Mappings](README.md): Linux OS Syslog - Process usermod - Change User ID

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Linux|
|Product|Syslog|
|Log Format|JSON|
|Event ID Regex Pattern|`usermod-change-id`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Linux|
|Product|Linux OS Syslog|
|Record Type|AuditChange|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|baseImage|syslog_process||
|changeTarget|user||
|device_hostname|syslog_hostname||
|pid|syslog_process_id||
|targetUser_username|user||
|user_userId|old_id||
|user_username|user||

