# [Mappings](README.md): cisco12

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCOFW302013_302014_302015_302016](../legacy_parsers/CISCOFW302013_302014_302015_302016.md)|

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
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `MMM dd yyyy HH:mm:ss`|
|user_username|user||

