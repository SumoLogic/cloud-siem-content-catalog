# [Mappings](README.md): Linux-Sysmon/Operational - 2

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Linux|
|Product|Sysmon|
|Log Format|Windows|
|Event ID Regex Pattern|`Linux-Sysmon/Operational-2`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Linux|
|Product|Sysmon for Linux|
|Record Type|EndpointProcess|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|None|The static text `A process changed a file creation time` is populated in this schema field.|
|baseImage|Image||
|description|None|The static text `Sysmon observed a process changed a file creation time` is populated in this schema field.|
|device_hostname|System.Computer||
|file_path|TargetFilename||
|sourceUid|System.EventRecordID||
|timestamp|UtcTime|We expect the orginal record value of `UtcTime` is in the format `yyyy-MM-dd HH:mm:ss.SSS`|
|user_userId|System.Security.UserId||
|user_username|User||

