# [Mappings](README.md): Unifi HTTP Request Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Log Format|JSON|
|Event ID Regex Pattern|`HTTP Request Event`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Ubiquiti|
|Product|Unifi|
|Record Type|NetworkHTTP|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|msg||
|device_hostname|syslog_hostname||
|errorText|error||
|http_method|request_type||
|http_url|request_url||
|pid|process_id||

