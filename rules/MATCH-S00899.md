# [Rules](README.md): Suspicious Active Directory Certificate Modification

## Description
This alert looks for an Active Directory certificate being modified with the "Any Purpose" OID. Threat actors may abuse this misconfiguration to forge certificates and Kerberos Ticket Granting Tickets (TGT). Specifically, this misconfiguration can exploit the "ESC2" attack path via https://posts.specterops.io/certified-pre-owned-d95910965cd2. If this event is deemed suspicious, look for authentication events (4624) that utilize this certificate template. Also ensure that this change was expected and approved within the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Suspicious Active Directory Certificate Modification|
|Summary Expression|Suspicious Active Directory Certificate Modification by {{user_username}}|
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
|Direct from Record|fields["EventData.AttributeValue"]|
|Direct from Record|fields["EventData.ObjectClass"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


