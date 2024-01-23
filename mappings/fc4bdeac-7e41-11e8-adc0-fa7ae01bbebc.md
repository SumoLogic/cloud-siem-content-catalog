# [Mappings](README.md): Trend Micro CEF logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Trend Micro|
|Product|Deep Security Manager|
|Log Format|CEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Trend Micro|
|Product|Deep Security|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|name||
|description|msg||
|device_hostname|host||
|device_ip|src||
|device_mac|src_mac||
|severity|severity||
|srcDevice_ip|src||
|user_username|target||

