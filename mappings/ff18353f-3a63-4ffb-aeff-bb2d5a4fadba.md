# [Mappings](README.md): Windows - WMI - 5680

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Windows|
|Log Format|Windows|
|Event ID Regex Pattern|`Microsoft-Windows-WMI-Activity/Operational-5860`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|commandLine|UserData.Operation_TemporaryEssStarted.Query||
|description|RenderingInfo.Message||
|device_hostname|Computer||
|timestamp|TimeCreated.SystemTime|We expect the orginal record value of `TimeCreated.SystemTime` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ`|
|user_userId|Security.UserID||
|user_username|UserData.Operation_TemporaryEssStarted.User||

