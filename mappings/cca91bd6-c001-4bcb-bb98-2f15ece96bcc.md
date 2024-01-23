# [Mappings](README.md): Alert

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Claroty|
|Product|Claroty xDome|
|Log Format|JSON|
|Event ID Regex Pattern|`alert_affected_device`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Claroty|
|Product|Claroty xDome|
|Record Type|Notification|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|alert_description||
|device_ip|device_ip||
|device_mac|device_mac||
|device_osName|device_os||
|severity|severity||
|threat_name|alert_description||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|alert_type_name||

