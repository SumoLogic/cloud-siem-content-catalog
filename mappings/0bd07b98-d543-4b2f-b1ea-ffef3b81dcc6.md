# [Mappings](README.md): Azure Event Hub - Windows Defender Authentication events

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Azure|
|Log Format|JSON|
|Event ID Regex Pattern|`AdvancedHunting-(IdentityLogonEvents\|DeviceLogonEvents)`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Azure|
|Record Type|Authentication|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|tenantId||
|action|properties.ActionType||
|application|properties.Application||
|cause|properties.FailureReason||
|device_hostname|properties.DeviceName||
|device_ip|properties.IPAddress||
|device_osName|properties.OSPlatform||
|device_type|properties.DeviceType||
|dstDevice_hostname|properties.DestinationDeviceName||
|dstDevice_ip|properties.DestinationIPAddress||
|dstPort|properties.DestinationPort||
|errorText|properties.FailureReason||
|ipProtocol|properties.Protocol||
|logonType|properties.LogonType||
|normalizedAction|None|The static text `logon` is populated in this schema field.|
|normalizedCause|properties.FailureReason|This is a lookup field. More info to come in the catalog later...|
|srcDevice_hostname|properties.DeviceName||
|srcDevice_ip|properties.IPAddress||
|srcPort|properties.Port||
|success|properties.ActionType|This is a lookup field. More info to come in the catalog later...|
|targetUser_email|properties.TargetAccountUpn||
|targetUser_username|properties.TargetAccountDisplayName||
|user_email|properties.AccountUpn||
|user_userId|properties.AccountSid||
|user_username|properties.AccountName||

