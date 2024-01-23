# [Rules](README.md): XSD Autostart Entry Modification

## Description
Observes for modifications to XSD Autostart entries which can be used to execute malicious programs at startup.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|XSD Autostart Entry Modification|
|Summary Expression|Detected XSD modification on host: {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547.013|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


