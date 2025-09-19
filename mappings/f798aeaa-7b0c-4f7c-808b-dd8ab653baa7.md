# [Mappings](README.md): TippingPoint TPS Cloud Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|TippingPoint|
|Product|TPS Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|TippingPoint|
|Product|TPS Cloud|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|device_hostname|syslog_hostname||
|device_ip|dvc||
|dstDevice_hostname|dvchost||
|dstDevice_ip|dst||
|dstPort|dpt||
|normalizedAction|act|This is a lookup field. More info to come in the catalog later...|
|srcDevice_hostname|srchost||
|srcDevice_ip|src||
|srcPort|spt||

