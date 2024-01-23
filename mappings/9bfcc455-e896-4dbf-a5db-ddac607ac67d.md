# [Mappings](README.md): Microsoft Cloud App Security - Direct

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|MCAS|
|Product|SIEM_Agent|
|Log Format|CEF|
|Event ID Regex Pattern|`^(?!ALERT_MANAGEMENT_GENERIC$)ALERT_.*$`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Cloud App Security|
|Record Type|Notification|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|msg||
|device_ip|src||
|normalizedSeverity|severity|This is a lookup field. More info to come in the catalog later...|
|severity|severity||
|threat_name|name||
|threat_referenceUrl|cs1||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|msg||
|timestamp|rt|We expect the orginal record value of `rt` is in the format `epoch`|
|user_username|suser||

