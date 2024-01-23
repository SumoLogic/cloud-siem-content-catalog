# [Mappings](README.md): Symantec Web Security Service C2C

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Symantec|
|Product|Web Security Service|
|Log Format|JSON|
|Event ID Regex Pattern|`proxy-messages`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Symantec|
|Product|Web Security Service|
|Record Type|NetworkProxy|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|x-bluecoat-request-tenant-id||
|action|s-action||
|bytesIn|cs-bytes||
|bytesOut|sc-bytes||
|device_hostname|x-bluecoat-appliance-name||
|device_ip|s-ip||
|dstDevice_ip|r-ip||
|dstPort|cs-uri-port||
|http_category|cs-categories||
|http_hostname|cs-host||
|http_method|cs-method||
|http_url|https://%s%s||
|srcDevice_ip|c-ip||

