# [Mappings](README.md): Trend Micro Control Manager CEF AV

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Trend Micro|
|Product|Control Manager|
|Log Format|CEF|
|Event ID Regex Pattern|`AV:.*`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Trend Micro|
|Product|Control Manager|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|device_hostname|dhost||
|device_ip|dst||
|file_basename|fname||
|file_path|filePath||
|normalizedSeverity|severity|This is a lookup field. More info to come in the catalog later...|
|severity|severity||
|success|act|This is a lookup field. More info to come in the catalog later...|
|threat_name|name||
|threat_ruleType|None|The static text `malware` is populated in this schema field.|
|timestamp|rt|We expect the orginal record value of `rt` is in the format `MMM dd yyyy HH:mm:ss zzzZ`|
|user_username|duser||

