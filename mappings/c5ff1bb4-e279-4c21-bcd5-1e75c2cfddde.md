# [Mappings](README.md): Cyber Ark EPM Policy

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cyber-Ark|
|Product|EPM|
|Log Format|JSON|
|Event ID Regex Pattern|`Policy`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cyber-Ark|
|Product|Endpoint Privilege Manager|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|Action||
|changeTarget|Platform||
|changeType|PolicyType||
|description|ComputerName||
|resource|PolicyId||

