# [Mappings](README.md): Cyber Ark EPM GetComputer

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cyber-Ark|
|Product|EPM|
|Log Format|JSON|
|Event ID Regex Pattern|`GetComputer`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cyber-Ark|
|Product|Endpoint Privilege Manager|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|Status||
|baseImage|Platform||
|description|ComputerType||
|dstDevice_hostname|ComputerName||
|dstDevice_uniqueId|AgentId||

