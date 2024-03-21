# [Mappings](README.md): Cato Networks Security Events - Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cato Networks|
|Product|Cato Networks|
|Log Format|JSON|
|Event ID Regex Pattern|`Connectivity\|System\|Routing\|Sockets Management`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cato Networks|
|Product|Cato Networks|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|account_id||
|action|action||
|application|application||
|device_osName|os_type||
|dstDevice_ip|dest_ip||
|dstPort|dest_port||
|http_hostname|domain_name||
|ipProtocol|ip_protocol||
|resource|event_type||
|resourceType|event_sub_type||
|srcDevice_ip|src_ip||
|user_email|vpn_user_email||
|user_username|src_site||

