# [Rules](README.md): Windows - Denied RDP

## Description
Generates a signal when windows event ID 4825 is observed. This indicates the user was denied an attempt to RDP.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|{{user_username}} was denied the access to Remote Desktop|
|Summary Expression|"{{user_username}}" was denied the access to Remote Desktop on "{{dstDevice_hostname}}" from "{{srcDevice_ip}}"|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1212|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


