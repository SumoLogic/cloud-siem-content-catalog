# [Rules](README.md): First Seen IP Address Connecting to Active Directory Certificate Services Process

## Description
This alert looks at Windows Filtering Platform Events and flags when a first seen IP address connects to the certificate services process. This can be indictive of enumeration of certificate templates which can potentially lead to forged certificates and privilege escalation avenues. Pivot off the source IP and ensure that this device is authorized to be on the network. In addition, look for other CSE signals related to Active Directory Certificate Services to look for any potentially vulnerable certificate templates being exploited.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, srcDevice_ip|
|Signal Name|First Seen IP Address Connecting to Active Directory Certificate Services Process from {{srcDevice_ip}} on {{device_hostname}}|
|Summary Expression|First Seen IP Address Connecting to Active Directory Certificate Services Process on {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1649, _mitreAttackTechnique:T1087.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


