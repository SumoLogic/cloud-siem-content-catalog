# [Mappings](README.md): 1Password Item Audit Actions

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|1Password|
|Product|1Password|
|Log Format|JSON|
|Event ID Regex Pattern|`audit.*`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|1Password|
|Product|1Password|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|action||
|application|client.app_name||
|srcDevice_ip|client.ip_address||
|srcDevice_osName|client.os_name||
|success|category|This is a lookup field. More info to come in the catalog later...|
|targetUser_email|target_user.email||
|targetUser_userId|target_user.uuid||
|targetUser_username|target_user.name||

