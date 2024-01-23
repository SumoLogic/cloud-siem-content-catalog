# [Mappings](README.md): Juniper SSG Series Firewall - Audit Messaging

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Juniper|
|Product|SSG Series Firewall|
|Log Format|JSON|
|Event ID Regex Pattern|`Audit`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Juniper|
|Product|SSG Series Firewall|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|alert||
|dstDevice_ip|dst||
|ipProtocol|proto|This is a lookup field. More info to come in the catalog later...|
|severity|type||
|srcDevice_ip|src||
|threat_identifier|type_id||
|threat_name|alert||
|timestamp|syslog_timestamp|We expect the orginal record value of `syslog_timestamp` is in the format `yyyy-MM-dd'T'HH:mm:ss`|

