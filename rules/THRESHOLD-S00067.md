# [Rules](README.md): ZeroLogon Privilege Escalation Behavior

## Description
An attack against CVE-2020-1472 may create thousands of NetrServerReqChallenge & NetrServerAuthenticate3 requests in a short amount of time. https://github.com/SecuraBV/CVE-2020-1472

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, dstDevice_ip, user_username|
|Signal Name|ZeroLogon Privilege Escalation Behavior|
|Summary Expression|Detected ZeroLogon privilege escalation behavior from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}}|
|Threshold Count|100|
|Threshold Window|5m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.005|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_dceRpc_endpoint|
|Normalized Schema|bro_dceRpc_operation|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


