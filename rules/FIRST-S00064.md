# [Rules](README.md): First Seen Certificate Thumbprint in Successful Kerberos Authentication

## Description
This alert looks for a first seen certtificate thumbprint being used to authenticate to an Active Directory environment, resulting in a Kerberos ticket being successfully issued. This alert is designed to catch Active Directory Certificate Services related attacks, ensure the certificate thumprint is valid, correlate the thumbprint ID with other Certificate Services events, particularly looking for recently issued templates.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Certificate Thumbprint in Successful Kerberos Authentication on {{device_hostname}}|
|Summary Expression|First Seen Certificate Thumbprint in Successful Kerberos Authentication on {{device_hostname}} by {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
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
|Direct from Record|fields["EventData.CertThumbprint"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


