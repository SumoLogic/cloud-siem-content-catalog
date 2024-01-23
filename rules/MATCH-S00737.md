# [Rules](README.md): Network Connection from MSHTA - Sysmon

## Description
Native Window utilities are often employed by attackers to execute malicious code in order to abuse the elevated privileges of these processes and to blend in with normal system activity. This rule monitors for outbound TCP/UDP connections spawning from mshta.exe as this could indicate a second-stage payload acquisition. Note that sysmon event ID 3 does not record ICMP connections.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, srcDevice_hostname, srcDevice_ip|
|Signal Name|Network Connection from MSHTA - Sysmon|
|Summary Expression|Mshta.exe made a network connection on host: {{srcDevice_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218, _mitreAttackTechnique:T1218.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


