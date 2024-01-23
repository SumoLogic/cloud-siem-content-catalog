# [Rules](README.md): Successful Overpass the Hash Attempt

## Description
Identifies a suspicious windows logon of type 9 (NewCredentials).  This signal is suspicious due to its similarity to the behavior observed when using Mimikatz's sekurlsa::pth tool.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Successful Overpass the Hash Attempt|
|Summary Expression|Successful Overpass the Hash attempted on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550, _mitreAttackTechnique:T1550.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.AuthenticationPackage']|
|Direct from Record|fields['EventData.AuthenticationPackageName']|
|Normalized Schema|logonType|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


