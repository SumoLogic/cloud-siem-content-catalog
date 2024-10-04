# [Mappings](README.md): McAfee WebGateway - CEF - User Login Failed

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|McAfee|
|Product|WebGateway|
|Log Format|CEF|
|Event ID Regex Pattern|`USER_LOGIN_FAILED`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|McAfee|
|Product|Web Gateway|
|Record Type|Authentication|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|cause|Details||
|description|None|The static text `A user failed authentication to the web gateway` is populated in this schema field.|
|device_hostname|Appliance||
|normalizedAction|None|The static text `logon` is populated in this schema field.|
|srcDevice_ip|Source_ID||
|success|None|The static text `false` is populated in this schema field.|
|timestamp|Timestamp|We expect the orginal record value of `Timestamp` is in the format `dd/MMM/yyyy:HH:mm:ss.SSS`|
|user_username|User||

