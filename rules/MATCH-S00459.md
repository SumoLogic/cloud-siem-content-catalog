# [Rules](README.md): Potential Cobalt Strike Profile

## Description
From FireEye Red Team Tool Countermeasures: This IOC detects indicators associated with cobalt strike beacon network activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_ip, srcDevice_ip, dstDevice_ip, device_hostname, srcDevice_hostname, dstDevice_hostname, user_username|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - Potential Cobalt Strike Profile|
|Summary Expression|Cobalt Strike Indicators detected on host: {{srcDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1029, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1567, _mitreAttackTechnique:T1567.001, _mitreAttackTechnique:T1567.002|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_url|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|parentBaseImage|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


