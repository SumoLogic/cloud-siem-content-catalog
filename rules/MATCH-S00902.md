# [Rules](README.md): Suspicious Active Directory Certificate Modification - Enrollment Agent

## Description
This alert looks for an Active Directory certificate being modified with an Enrollment Agent value that allows an Active Directory principal to enroll a certificate on behalf of another user. Threat actors may abuse this misconfiguration to forge certificates and Kerberos Ticket Granting Tickets (TGT). Specifically, this misconfiguration can exploit the "ESC3" attack path via https://posts.specterops.io/certified-pre-owned-d95910965cd2. If this event is deemed suspicious, look for authentication events (4624) that utilize this certificate template. Also ensure that this change was expected and approved within the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|Suspicious Active Directory Certificate Modification - Enrollment Agent by {{user_username}}|
|Summary Expression|Suspicious Active Directory Certificate Modification - Enrollment Agent by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1649|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cepencryption|
|Normalized Schema|certificate|
|Normalized Schema|device_hostname|
|Normalized Schema|enrollmentagent|
|Normalized Schema|enrollmentagentoffline|
|Direct from Record|fields["EventData.AttributeValue"]|
|Direct from Record|fields["EventData.ObjectClass"]|
|Direct from Record|fields["EventData.ObjectDN"]|
|Normalized Schema|machineenrollmentagent|
|Normalized Schema|matches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


