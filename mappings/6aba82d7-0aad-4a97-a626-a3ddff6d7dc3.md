# [Mappings](README.md): F5 TMSH - Custom Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|F5|
|Product|F5|
|Log Format|JSON|
|Event ID Regex Pattern|`tmsh`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|F5|
|Product|F5|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|device_hostname|syslog_hostname||
|normalizedSeverity|syslog_severity|This is a lookup field. More info to come in the catalog later...|
|pid|pid||
|severity|syslog_severity||
|success|status|This is a lookup field. More info to come in the catalog later...|
|user_username|user||

