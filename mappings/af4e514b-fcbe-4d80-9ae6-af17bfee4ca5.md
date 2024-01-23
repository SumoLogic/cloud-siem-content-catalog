# [Mappings](README.md): Trend Micro CEF logs - Integrity Monitoring

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Trend Micro|
|Product|Deep Security Manager|
|Log Format|CEF|
|Event ID Regex Pattern|`^2[0-9]{6}$`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Trend Micro|
|Product|Deep Security|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|msg||
|device_ip|src||
|normalizedSeverity|severity|This is a lookup field. More info to come in the catalog later...|
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|name||
|user_username|suser||

