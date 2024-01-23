# [Rules](README.md): Potential Microsoft Office In-Memory Token Theft

## Description
Office applications and Web Browsers connecting to Office services can potentially store credential material in their memory space. This event indicates that a process has accessed the memory space of an Office process that may potentially contain token material.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Microsoft Office In-Memory Token Theft|
|Summary Expression|{{device_hostname}} has logged a suspicious process access event potentially indicating in-memory credential or token theft from an Office application.|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555.003, _mitreAttackTechnique:T1003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields["EventData.CallTrace"]|
|Direct from Record|fields["EventData.GrantedAccess"]|
|Direct from Record|fields["EventData.SourceImage"]|
|Normalized Schema|matches|
|Normalized Schema|metadata_deviceEventId|


