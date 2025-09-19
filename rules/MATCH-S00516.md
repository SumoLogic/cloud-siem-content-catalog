# [Rules](README.md): Antivirus Ransomware Detection

## Description
Malware detected that is determined to be ransomware based on the signature/virus name.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Antivirus Ransomware Detection|
|Summary Expression|{{threat_name}} detected on host: {{device_hostname}}|
|Score/Severity|Static: 8|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1542, _mitreAttackTechnique:T1105, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.002, _mitreAttackTechnique:T1562.003, _mitreAttackTechnique:T1562.004, _mitreAttackTechnique:T1562.006, _mitreAttackTechnique:T1562.001, _mitreAttackTechnique:T1562.002, _mitreAttackTechnique:T1484.001|
## Vendors and Products
- [Cisco Systems - Advanced Malware Protection (AMP)](../products/7eaa4c44-5b7f-4d9e-8c1c-c4105c2b7506.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [McAfee - Endpoint Security](../products/c91067a3-e972-4a73-ac14-75df12d49cc8.md)
- [Symantec - Endpoint Protection](../products/eb2f69a8-8d13-447f-9859-1ad0979b4a24.md)
- [Trend Micro - Control Manager](../products/bb75c481-648d-4953-80cf-1c8cbde8fbb8.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|threat_name|
|Normalized Schema|threat_ruleType|
|Normalized Schema|user_username|


