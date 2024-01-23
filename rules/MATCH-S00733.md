# [Rules](README.md): Registry Modification - Print Processors

## Description
Observes for modifications to registry entries defining print processors for the print spooler service. The print spooler runs with  system level permissions and this technique can be used to establish persistence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname|
|Signal Name|Registry Modification - Print Processors|
|Summary Expression|Print Processor modified on host: {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1547, _mitreAttackTactic:TA0003, _mitreAttackTechnique:T1547.012|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|


