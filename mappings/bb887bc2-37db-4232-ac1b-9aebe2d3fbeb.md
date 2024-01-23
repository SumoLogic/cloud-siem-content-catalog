# [Mappings](README.md): Linux OS Syslog - Process su - Switch User

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Linux|
|Product|Syslog|
|Log Format|JSON|
|Event ID Regex Pattern|`su`|

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
|changeTarget|switched_user||
|device_hostname|syslog_hostname||
|pid|syslog_process_id||
|success|outcome|This is a lookup field. More info to come in the catalog later...|
|targetUser_username|switched_user||
|user_userId|uid||
|user_username|original_user||

