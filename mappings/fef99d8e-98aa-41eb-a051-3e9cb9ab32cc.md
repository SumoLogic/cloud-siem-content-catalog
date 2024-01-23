# [Mappings](README.md): Cisco Meraki Catch All - Custom Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|Meraki|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Meraki|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|decision||
|dstDevice_ip|dst||
|dstPort|dport||
|ipProtocol|protocol||
|srcDevice_ip|src||
|srcPort|sport||
|timestamp|syslog_timestamp|We expect the orginal record value of `syslog_timestamp` is in the format `epoch_float`|

