# [Mappings](README.md): Unifi Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|commandLine|command||
|description|msg||
|device_hostname|syslog_hostname||
|device_uniqueId|device_id||
|dstDevice_ip|dst_ip||
|dstPort|nameserver_port||
|errorText|error_message||
|http_url|url||
|ipProtocol|protocol||
|normalizedAction|action|This is a lookup field. More info to come in the catalog later...|
|pid|process_id||
|success|status|This is a lookup field. More info to come in the catalog later...|

