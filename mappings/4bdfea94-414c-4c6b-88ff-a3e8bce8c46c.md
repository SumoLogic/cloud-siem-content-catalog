# [Mappings](README.md): Citrix Cloud Operation Logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Citrix|
|Product|Cloud|
|Log Format|JSON|
|Event ID Regex Pattern|`Operation Logs`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Citrix|
|Product|Cloud|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|OperationType||
|description|Text||
|device_ip|AdminMachineIP||
|resourceType|TargetTypes||
|success|IsSuccessful||
|user_email|User||
|user_role|Source||

