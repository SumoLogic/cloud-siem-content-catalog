# [Rules](README.md): Unsigned Image Loaded by LSASS

## Description
Detects an unsigned image being loaded by LSASS as this may indicate attempted credential access. This rule may also detect persistence activity via LSASS driver loads.

Note that this rule requires Microsoft SysInternals Sysmon installed with Image Loaded (Event Id 7) logging enabled.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Unsigned Image Loaded by LSASS|
|Summary Expression|Unsigned image loaded: {{baseImage}} on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.001, _mitreAttackTechnique:T1547.008|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['EventData.Signed']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


