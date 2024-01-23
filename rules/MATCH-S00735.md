# [Rules](README.md): Registry Modification - SIP or Trust Provider

## Description
Trust Providers and Subject Interface Packages (SIPs) can be modified via the Windows Registry to allow attackers to execute malicious code with heightened permissions and less oversight. This rule monitors for changes to several Registry keys containing values that modify these settings.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Registry Modification - SIP or Trust Provider|
|Summary Expression|User {{user_username}} modified registry key {{changeTarget}} on host {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1553.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


