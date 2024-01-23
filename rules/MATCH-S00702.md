# [Rules](README.md): Keychain Credential Dumping

## Description
Attackers may dump the content of the keychain storage data from a system to acquire credentials.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Keychain Credential Dumping|
|Summary Expression|Keychain Credential Dumping Detected on host: {{device_hostname}} IP: {{device_ip}} with user: {{user_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555, _mitreAttackTechnique:T1555.001, _mitreAttackTechnique:T1555.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


