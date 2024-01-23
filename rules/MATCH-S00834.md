# [Rules](README.md): Sensitive Registry Key (WDigest) Edit

## Description
Enabling of Wdigest authentication may enable the storage of plain text credential material on Windows systems. WDigest is disabled by default on newer versions of Windows systems, manual enablement of this registry key may indicate suspicious activity and attempts at credential theft.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname|
|Signal Name|Sensitive Registry Key (WDigest) Edit|
|Summary Expression|The {{changeTarget}} registry key has been enabled on {{device_hostname}}|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1112, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003.001|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|resource|


