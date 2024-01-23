# [Mappings](README.md): Netskope - Anomaly - Bulk Download

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Netskope|
|Product|Security Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`bulk_download`|

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
|device_ip|userip||
|device_natIp|srcip||
|file_basename|object||
|file_hash_md5|md5||
|threat_name|alert||
|user_username|user||

