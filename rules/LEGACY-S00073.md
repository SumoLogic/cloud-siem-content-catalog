# [Rules](README.md): SMB External to Internal File Share Access

## Description
This signal identifies external sources connecting to file shares.  Do to the vulnerabilities and insecurities of SMB this type of traffic should be prohibited. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SMB External to Internal File Share Access|
|Summary Expression|External IP: {{srcDevice_ip}} connecting to internal file share on IP: {{srcDevice_ip}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_smb_file.action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


