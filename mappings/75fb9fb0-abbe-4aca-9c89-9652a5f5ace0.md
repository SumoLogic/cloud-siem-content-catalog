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
|dstDevice_ip|dst_ip||
|dstPort|dst_port||
|normalizedAction|action|This is a lookup field. More info to come in the catalog later...|
|srcDevice_ip|src_ip||
|srcPort|src_port||
|user_username|user||

