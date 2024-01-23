# [Rules](README.md): SYSVOL Share Sweep

## Description
When attempting to pivot within an internal AD network, attacks will query the Domain Controllers for passwords stored within group policy files. This is typically done by querying the SYSVOL share.  A host querying the SYSVOL share is suspicious activity and could be indicative of this type of attack.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SYSVOL Share Sweep|
|Summary Expression|SYSVOL share sweep on host: {{device_hostname}}|
|Threshold Count|5|
|Threshold Window|5m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1135|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


