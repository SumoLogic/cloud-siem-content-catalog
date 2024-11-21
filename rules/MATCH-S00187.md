# [Rules](README.md): Process Execution Inside Webserver Root Folder

## Description
A process was executed from inside a web hosting directory. This signal could indicate when adversaries upload a malicious file to the webserver and run the file as a process. Approved web applications that require process execution from inside the web hosting directory should be excluded from the rule and filtered out.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Process Execution Inside Webserver Root Folder|
|Summary Expression|Process executed in web host directory: {{baseImage}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0002, _mitreAttackTechnique:T1190, _mitreAttackTechnique:T1203|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


