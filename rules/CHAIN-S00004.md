# [Rules](README.md): Lateral Movement Using the Windows Hidden Admin Share

## Description
Detects pivoting to an internal host from another internal host. Attackers will connect to the ADMIN$ share of an internal host and upload a program to execute remote commands to fully compromise the host.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname|
|Signal Name|Lateral Movement Using the Windows Hidden Admin Share|
|Summary Expression|Lateral movement detected to host: {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


