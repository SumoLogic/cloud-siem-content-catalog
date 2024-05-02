# [Rules](README.md): Potentially Misconfigured Active Directory Certificate Template Loaded

## Description
This alert looks at Active Directory Certificate Services Auditing Events to look for a certificate template issued that allows all domain users the ability to enroll the template. Combined with other misconfigurations within a certificate template, this can potentially allow a threat actor to turn a certificate obtained from such a vulnerable template into a Kerberos Ticket Granting Ticket (TGT) which could enable privilege escalation paths.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potentially Misconfigured Active Directory Certificate Template Loaded on {{device_hostname}}|
|Summary Expression|Potentially Misconfigured Active Directory Certificate Template Loaded on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1649|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|


