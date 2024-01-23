# [Mappings](README.md): OpenVPN Logon Attempt

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|OpenVPN|
|Product|OpenVPN|
|Log Format|JSON|
|Event ID Regex Pattern|`AUTH_(FAILED\|SUCCESS)`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|OpenVPN|
|Product|OpenVPN|
|Record Type|Authentication|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|description||
|errorCode|status||
|errorText|reason||
|normalizedAction|None|The static text `logon` is populated in this schema field.|
|srcDevice_ip|src_ip||
|srcPort|src_port||
|success|message_type|This is a lookup field. More info to come in the catalog later...|
|user_username|user||

