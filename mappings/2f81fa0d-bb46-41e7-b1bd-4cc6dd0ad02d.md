# [Mappings](README.md): Imperva Incapsula Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Imperva|
|Product|Imperva Incapsula|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Imperva|
|Product|Imperva Incapsula|
|Record Type|NetworkHTTP|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|http_method|requestMethod||
|http_url|request||
|http_userAgent|requestClientApplication||
|srcDevice_ip|src||
|srcPort|spt||
|timestamp|start|We expect the orginal record value of `start` is in the format `epoch`|

