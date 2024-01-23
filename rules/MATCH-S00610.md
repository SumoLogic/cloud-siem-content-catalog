# [Rules](README.md): PSExec Named Pipe Created by Non-PsExec Process

## Description
Observes for creation of a PSExec named pipe not by PSExec. This may be an indication of a malicious process coopting a privileged named pipe used by PSExec.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|PSExec Named Pipe Created by Non-PsExec Process|
|Summary Expression|Observed the creation of a PSExec named pipe by a non-PsExec process on {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.002, _mitreAttackTechnique:T1021.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


