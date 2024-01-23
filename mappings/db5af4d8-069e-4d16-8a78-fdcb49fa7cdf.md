# [Mappings](README.md): Windows - System - 6006

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Windows|
|Log Format|Windows|
|Event ID Regex Pattern|`System-6006`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|None|The static text `The event log service was stopped` is populated in this schema field.|
|device_hostname|Computer||
|timestamp|TimeCreated.SystemTime|We expect the orginal record value of `TimeCreated.SystemTime` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ`|

