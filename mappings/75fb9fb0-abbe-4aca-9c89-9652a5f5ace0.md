# [Mappings](README.md): OpenVPN Network Event

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|OpenVPN|
|Product|OpenVPN|
|Log Format|JSON|
|Event ID Regex Pattern|`network`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|OpenVPN|
|Product|OpenVPN|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|description|event||
|device_hostname|host||
|srcDevice_ip|src_ip||
|srcPort|src_port||
|user_username|user||

