# [Rules](README.md): DNS RCE Exploit CVE-2020-1350

## Description
Detects exploitation of DNS RCE bug reported in CVE-2020-1350 by the detection of suspicious sub process

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|DNS RCE Exploit CVE-2020-1350|
|Summary Expression|Potential Remote Code Execution on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0002, _mitreAttackTechnique:T1190, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1569.002|
## Vendors and Products
- [Bitdefender - GravityZone](../products/046b3623-69fe-409f-9e80-fd3ebef0654f.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


