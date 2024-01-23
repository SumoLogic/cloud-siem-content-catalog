# [Rules](README.md): Malware Outbreak

## Description
Detects the same malware signature on multiple hosts in a short timeframe. This indicates malware may be spreading in the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Malware Outbreak|
|Summary Expression|Malware: {{threat_name}} cleaned on multiple hosts|
|Threshold Count|5|
|Threshold Window|30m|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1204, _mitreAttackTechnique:T1569.002, _mitreAttackTechnique:T1204.002, _mitreAttackTechnique:T1204.003|
## Vendors and Products
- [Bitdefender - GravityZone](../products/046b3623-69fe-409f-9e80-fd3ebef0654f.md)
- [Cisco Systems - Advanced Malware Protection (AMP)](../products/7eaa4c44-5b7f-4d9e-8c1c-c4105c2b7506.md)
- [Cybereason - Endpoint Security](../products/12d00042-d90d-4055-a171-01a1f635a613.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [McAfee - Endpoint Security](../products/c91067a3-e972-4a73-ac14-75df12d49cc8.md)
- [Symantec - Endpoint Protection](../products/eb2f69a8-8d13-447f-9859-1ad0979b4a24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|threat_name|
|Normalized Schema|threat_ruleType|
|Normalized Schema|user_username|


