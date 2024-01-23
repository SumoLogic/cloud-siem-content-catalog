# [Rules](README.md): Powerview Add-DomainObjectAcl DCSync AD Extend Right

## Description
Backdooring domain object to grant the rights associated with DCSync to a regular user or machine account using Powerview\Add-DomainObjectAcl DCSync Extended Right cmdlet, will allow to re-obtain the pwd hashes of any user/computer

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Powerview Add-DomainObjectAcl DCSync AD Extend Right|
|Summary Expression|Detected Powerview Add-DomainObjectAcl DCSync AD Extend Right use on {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1059, _mitreAttackTechnique:T1059.001, _mitreAttackTechnique:T1059.003, _mitreAttackTechnique:T1003, _mitreAttackTechnique:T1003.006|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['EventData.AttributeLDAPDisplayName']|
|Direct from Record|fields['EventData.AttributeValue']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


