# [Rules](README.md): ADPassHunt Tool

## Description
From FireEye Red Team Tool Countermeasures:
This IOC detects indicators associated with the ADPassHunt Tool. This tool is used to hunt for AD credentials and used via execute-assembly that looks for passwords in GPP, Autoruns and AD objects

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|FireEye ADPassHunt Tool|
|Summary Expression|ADPassHunt (credential stealer) tool associated command line arguments detected on host: {{device_hostname}} by user: {{user_username}} using process: {{baseImage}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.006, _mitreAttackTechnique:T1003.005|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


