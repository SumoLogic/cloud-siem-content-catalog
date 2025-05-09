# [Mappings](README.md): Cisco Umbrella DNS Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|Umbrella|
|Log Format|JSON|
|Event ID Regex Pattern|`dnslogs`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Umbrella|
|Record Type|NetworkDNS|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|description|categories||
|dns_query|domain||
|dns_queryDomain|domain||
|dns_queryType|query_type||
|dns_returnCode|dnsReturnCode||
|dstDevice_ip|dstdeviceIP||
|http_category|categories||
|normalizedAction|action|This is a lookup field. More info to come in the catalog later...|
|srcDevice_hostname|Anyconnect Roaming Client||
|srcDevice_ip|internal_ip||
|timestamp|timestamp|We expect the orginal record value of `timestamp` is in the format `yyyy/MM/dd HH:mm:ss`|
|user_email|email_address||
|user_username|email_address|This is a split field. More info to come in the catalog later...|

