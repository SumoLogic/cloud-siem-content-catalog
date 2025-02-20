# [Mappings](README.md): Netskope - Anomaly - Bulk Download

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`(?i)(bulk_download\|bulk download)`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|activity||
|application|app||
|device_hostname|hostname||
|device_ip|userip||
|device_natIp|srcip||
|device_osName|os_version||
|dstDevice_ip|dstip||
|dstPort|dstport||
|file_basename|file_path||
|file_hash_md5|md5||
|http_category|category||
|http_referer|referer||
|http_url|url||
|http_userAgent|useragent||
|srcDevice_ip|srcip||
|threat_name|alert_name||
|user_email|user||
|user_username|user||

