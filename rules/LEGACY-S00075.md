# [Rules](README.md): SMB - Remote execution and/or persistence via scheduled task using ATSVC 

## Description
Remote execution and/or persistence via scheduled task using ATSVC named pipe.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SMB - Remote execution and/or persistence via scheduled task using ATSVC |
|Summary Expression|Remote execution via named pipe from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_smb_file.action|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


