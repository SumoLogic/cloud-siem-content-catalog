# [Mappings](README.md): Cisco Umbrella IP Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|Umbrella|
|Log Format|JSON|
|Event ID Regex Pattern|`iplogs`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Umbrella|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|dstDevice_ip|destination_ip||
|dstPort|destination_port||
|srcDevice_hostname|Anyconnect Roaming Client||
|srcDevice_ip|source_ip||
|srcPort|source_port||
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `yyyy/MM/dd HH:mm:ss`|
|user_email|email_address||
|user_username|email_address|This is a split field. More info to come in the catalog later...|

