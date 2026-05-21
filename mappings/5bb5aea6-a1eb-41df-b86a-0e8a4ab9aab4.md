# [Mappings](README.md): Claude - Admin API Key Events

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Anthropic|
|Product|Claude Activity Logs|
|Log Format|JSON|
|Event ID Regex Pattern|`admin_api_key_(created\|deleted\|updated)`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Anthropic|
|Product|Claude Activity Logs|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|----------------|-------------------|-----|
|accountId|organization_id||
|action|type||
|changeTarget|admin_api_key_id||
|changeType|type|This is a lookup field. More info to come in the catalog later...|
|cloud_provider|None|The static text `Anthropic` is populated in this schema field.|
|cloud_service|None|The static text `Claude` is populated in this schema field.|
|description|type|This is a lookup field. More info to come in the catalog later...|
|device_ip|actor.ip_address||
|http_userAgent|actor.user_agent||
|normalizedAction|type|This is a lookup field. More info to come in the catalog later...|
|normalizedResource|None|The static text `key` is populated in this schema field.|
|normalizedSeverity|type|This is a lookup field. More info to come in the catalog later...|
|resource|admin_api_key_id||
|srcDevice_ip|actor.ip_address||
|success|None|The static text `true` is populated in this schema field.|
|user_userId|actor.user_id||
|user_username|actor.email_address||

