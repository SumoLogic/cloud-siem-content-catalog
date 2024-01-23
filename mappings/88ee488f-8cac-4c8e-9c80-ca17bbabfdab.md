# [Mappings](README.md): Cisco ASA 113008 JSON

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|ASA|
|Log Format|JSON|
|Event ID Regex Pattern|`^113008$`|

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
|description|reason||
|severity|severity||
|success|None|The static text `false` is populated in this schema field.|
|user_username|user||

