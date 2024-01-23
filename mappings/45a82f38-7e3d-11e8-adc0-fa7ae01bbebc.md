# [Mappings](README.md): cisco2

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCOFW106006_106007_106010](../legacy_parsers/CISCOFW106006_106007_106010.md)|

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

