# [Mappings](README.md): Windows - Microsoft-Windows-Sysmon/Operational - 17

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Windows|
|Log Format|Windows|
|Event ID Regex Pattern|`Microsoft-Windows-Sysmon/Operational-17`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|EndpointProcess|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|None|The static text `PipeCreated` is populated in this schema field.|
|baseImage|EventData.Image||
|changeTarget|EventData.PipeName||
|description|None|The static text `Sysmon observed a pipe creation` is populated in this schema field.|
|device_hostname|Computer||
|normalizedAction|None|The static text `create` is populated in this schema field.|
|pid|EventData.ProcessId||
|resource|EventData.PipeName||
|sourceUid|EventRecordID||
|timestamp|EventData.UtcTime|We expect the orginal record value of `EventData.UtcTime` is in the format `yyyy-MM-dd HH:mm:ss.SSS`|
|user_userId|Security.UserID||

