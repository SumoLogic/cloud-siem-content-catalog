# [Mappings](README.md): Datto Asset Info Logs 1

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Datto|
|Product|S4E36|
|Log Format|CEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Datto|
|Product|SIRIS 4 Enterprise|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|device_hostname|dvchost||
|device_ip|dvc||
|timestamp|start|We expect the orginal record value of `start` is in the format `epoch`|

