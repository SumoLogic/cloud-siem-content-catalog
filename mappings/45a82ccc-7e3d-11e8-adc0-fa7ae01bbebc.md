# [Mappings](README.md): cisco1

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCOFW106001](../legacy_parsers/CISCOFW106001.md)|

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
|dstPort|dst_port||
|ipProtocol|protocol||
|srcDevice_ip|src_ip||
|srcPort|src_port||
|success|None|The static text `false` is populated in this schema field.|

