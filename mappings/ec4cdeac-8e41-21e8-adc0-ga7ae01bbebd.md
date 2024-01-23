# [Mappings](README.md): Trend Micro Control Manager CEF 700107

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Trend Micro|
|Product|Control Manager|
|Log Format|CEF|
|Event ID Regex Pattern|`700107`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Trend Micro|
|Product|Control Manager|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|device_hostname|shost||
|file_basename|fname||
|severity|severity||
|timestamp|rt|We expect the orginal record value of `rt` is in the format `MMM dd yyyy HH:mm:ss zzzZ`|

