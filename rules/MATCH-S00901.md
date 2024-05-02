# [Rules](README.md): Potentially Vulnerable Active Directory Certificate Services Template Loaded

## Description
This alert looks at Active Directory Certificate Services Auditing Events to look for a certificate template issued that allows the enrolee to supply a subject and allows all domain users to enroll. This combination allows a threat actor to turn a certificate obtained from a vulnerable template into a Kerberos Ticket Granting Ticket (TGT) which could enable privilege escalation paths. Specifically, this misconfiguration can exploit the "ESC1" attack path via https://posts.specterops.io/certified-pre-owned-d95910965cd2.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potentially Vulnerable Active Directory Certificate Services Template Loaded on {{device_hostname}}|
|Summary Expression|Potentially Vulnerable Active Directory Certificate Services Template Loaded from {{device_hostname}}|
|Score/Severity|Static: 4|
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


