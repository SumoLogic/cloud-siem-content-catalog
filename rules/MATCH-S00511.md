# [Rules](README.md): Accessibility Executables Replaced

## Description
Observes Sysmon 11 events for accessibility binaries being replaced

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Accessibility Executables Replaced|
|Summary Expression|The accessibility binary: {{file_path}} was observed being replaced on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1546, _mitreAttackTechnique:T1546.008|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_username|


