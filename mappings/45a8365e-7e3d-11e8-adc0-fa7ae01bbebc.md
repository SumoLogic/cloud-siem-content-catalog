# [Mappings](README.md): cisco5

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCOFW106021](../legacy_parsers/CISCOFW106021.md)|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|ASA|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|dstDevice_ip|dst_ip||
|ipProtocol|protocol||
|srcDevice_ip|src_ip||
|success|None|The static text `false` is populated in this schema field.|

