# [Mappings](README.md): Windows - Security - 4670

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Microsoft|
|Product|Windows|
|Log Format|Windows|
|Event ID Regex Pattern|`Security-4670`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Microsoft|
|Product|Windows|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|changeType|None|The static text `Permissions on an object were changed` is populated in this schema field.|
|description|None|The static text `Permissions on an object were changed` is populated in this schema field.|
|device_hostname|Computer||
|timestamp|TimeCreated.SystemTime|We expect the orginal record value of `TimeCreated.SystemTime` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSSSSSSSZ`|
|user_authDomain|EventData.SubjectDomainName||
|user_userId|EventData.SubjectUserSid||
|user_username|EventData.SubjectUserName||

