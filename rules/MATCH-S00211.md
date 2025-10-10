# [Rules](README.md): DNS.EXE Observed as Parent Process

## Description
With very few exceptions, the DNS.EXE program should not spawn other processes.  This could be an indication that the process is a trojan, or has been compromised.  This behavior against DNS has been shown as a behavioral indicator after successful attacks (i.e. SigRED).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip, user_username, device_hostname|
|Signal Name|DNS.EXE Observed as Parent Process|
|Summary Expression|DNS.exe spawned process {{baseImage}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


