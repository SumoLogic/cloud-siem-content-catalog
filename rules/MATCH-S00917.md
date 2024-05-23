# [Rules](README.md): Suspicious PowerShell Application Window Discovery COM method 

## Description
This PowerShell COM method allows for discovery of running application windows, along with the process path and window location coordinates.  Investigation of the host is recommended to identify the behavior leading to and around the execution of this PowerShell process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip|
|Signal Name|Suspicious PowerShell Application Window Discovery via COM method on {{device_hostname}}|
|Summary Expression|Suspicious use of Windows COM method via PowerShell  for Application Windows Discovery on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1010|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|


