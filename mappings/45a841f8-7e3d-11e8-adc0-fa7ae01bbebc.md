# [Mappings](README.md): cisco13

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCOFW302020_302021](../legacy_parsers/CISCOFW302020_302021.md)|

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
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `MMM dd yyyy HH:mm:ss`|
|user_username|user||

