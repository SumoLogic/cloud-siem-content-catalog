# [Mappings](README.md): Netskope - Network Events

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`network`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|activity||
|application|app||
|bytesIn|server_bytes||
|bytesOut|client_bytes||
|device_ip|userip||
|device_osName|device||
|dstDevice_hostname|dsthost||
|dstDevice_ip|dstip||
|dstPort|dstport||
|ipProtocol|ip_protocol||
|normalizedAction|action|This is a lookup field. More info to come in the catalog later...|
|packetsIn|server_packets||
|packetsOut|client_packets||
|srcDevice_hostname|srchost||
|srcDevice_ip|srcip||
|srcPort|srcport||
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `epoch`|
|user_email|user||
|user_username|user||

