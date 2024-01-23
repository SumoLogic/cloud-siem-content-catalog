# [Mappings](README.md): Windows - Security - 4714

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Windows|
|Log Format|Windows|
|Event ID Regex Pattern|`Security-4714`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|None|The static text `Encrypted data recovery policy was changed` is populated in this schema field.|
|device_hostname|Computer||
|timestamp|TimeCreated.SystemTime|We expect the orginal record value of `TimeCreated.SystemTime` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ`|

