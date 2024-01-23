# [Mappings](README.md): Cisco Meraki Security Filtering File Scanned

## Input Requirements

|Legacy Parser Grok Patterns|
|-------------|
|[CISCO_MERAKI_SECURITY_FILTERING_FILE_SCANNED](../legacy_parsers/CISCO_MERAKI_SECURITY_FILTERING_FILE_SCANNED.md)|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Meraki|
|Record Type|NetworkHTTP|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|dstDevice_ip|dst_ip||
|dstPort|dst_port||
|file_hash_sha256|sha256||
|http_url|url||
|ipProtocol|protocol||
|srcDevice_ip|src_ip||
|srcPort|src_port||
|timestamp|log_timestamp|We expect the orginal record value of `log_timestamp` is in the format `epoch_float`|

