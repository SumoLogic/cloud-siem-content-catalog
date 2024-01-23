# [Mappings](README.md): Palo Alto Threat URL Filtering - Custom Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Palo Alto|
|Product|Firewall|
|Log Format|JSON|
|Event ID Regex Pattern|`threat-url`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Palo Alto Networks|
|Product|Next Generation Firewall|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|application|application||
|device_hostname|firewall_name||
|dstDevice_ip|dest_ip||
|dstPort|dest_port||
|http_category|category||
|http_method|http_method||
|http_referer|http_referrer||
|http_requestHeaders|http_headers||
|http_url|http_url||
|http_userAgent|http_user_agent||
|ipProtocol|protocol||
|resource|flags||
|severity|pan_severity||
|srcDevice_ip|source_ip||
|srcPort|source_port||
|success|action|This is a lookup field. More info to come in the catalog later...|
|threat_category|threat_category||
|user_username|source_user||

