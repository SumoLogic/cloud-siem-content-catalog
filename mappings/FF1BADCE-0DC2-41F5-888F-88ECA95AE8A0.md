# [Mappings](README.md): Netskope - Infrastructure Events

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`infrastructure`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|alarm_name||
|device_hostname|device_name||
|severity|severity|This is a lookup field. More info to come in the catalog later...|
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `epoch`|
|user_username|user||

