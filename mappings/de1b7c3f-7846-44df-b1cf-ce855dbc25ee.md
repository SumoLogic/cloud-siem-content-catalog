# [Mappings](README.md): Juniper SRX Series Firewall - Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Juniper|
|Product|SRX Series Firewall|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Juniper|
|Product|SRX Series Firewall|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|reason||
|application|application||
|bytesIn|bytes-from-server||
|bytesOut|bytes-from-client||
|cause|reason||
|description|description||
|dstDevice_ip|destination-address||
|dstDevice_natIp|nat-destination-address||
|dstPort|destination-port||
|ipProtocol|protocol-id|This is a lookup field. More info to come in the catalog later...|
|packetsIn|packets-from-server||
|packetsOut|packets-from-client||
|srcDevice_ip|source-address||
|srcDevice_natIp|nat-source-address||
|srcPort|source-port||
|success|event_name|This is a lookup field. More info to come in the catalog later...|
|timestamp|reason|We expect the orginal record value of `reason` is in the format `yyyy-MM-dd'T'HH:mm:ss`|
|user_username|username||

