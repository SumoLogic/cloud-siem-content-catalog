# [Rules](README.md): Unsafe Outlook Rule Creation Enabled

## Description
Detects a registry modification that enables the creation of Outlook mail rules that can run scripts. This functionality is disabled by default. The addition of the EnableUnsafeClientMailRules registry entry is highly suspicious. This feature can be used by an adversary to establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Malicious Outlook Mail Rule Creation|
|Summary Expression|Unsafe Outlook Rule Creation Enabled on host: {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1137, _mitreAttackTechnique:T1137.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


