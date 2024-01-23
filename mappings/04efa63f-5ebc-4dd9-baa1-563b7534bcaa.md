# [Mappings](README.md): Cisco ASA 721016-8 JSON

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|ASA|
|Log Format|JSON|
|Event ID Regex Pattern|`^72101[68]$`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|ASA|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|severity|severity||
|srcDevice_ip|source_ip||
|success|None|The static text `true` is populated in this schema field.|
|user_username|user||

