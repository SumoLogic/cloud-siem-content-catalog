# [Rules](README.md): Cloud Credential File Accessed

## Description
When connecting to various cloud services using Azure PowerShell, Az PowerShell, AWS CLI, Google Cloud CLI or Kubeconfig, credential material may be left on the file system. Threat actors may read or exfiltrate this credential material in order to gain unauthroized access to various cloud resources from on premises hosts.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Cloud Credential File Accessed|
|Summary Expression|The file: {{file_path}} potentially containing cloud credentials (AWS, Kubeconfig, Azure, GCP) was accessed on {{device_hostname}} by user {{user_username}} via the process {{baseImage}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552.001, _mitreAttackTechnique:T1528|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


