# [Rules](README.md): Potential Active Directory Certificate Services Enrollment Agent Misconfiguration

## Description
This alert looks for two events in a particular order, the first event involves a certificate template being loaded with a certificate request agent application policy. The second event involves the same event type, but with a client authentication application policy. Together, these events may indicate exploitation of an “enrollment agent” misconfiguration. Threat actors may abuse this misconfiguration to forge certificates and Kerberos Ticket Granting Tickets (TGT). Specifically, this misconfiguration can exploit the "ESC3" attack path via https://posts.specterops.io/certified-pre-owned-d95910965cd2. If this event is deemed suspicious, look for authentication events (4624) that utilize this certificate template. Also ensure that this change was expected and approved within the environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Active Directory Certificate Services Enrollment Agent Misconfiguration|
|Summary Expression|Potential Active Directory Certificate Services Enrollment Agent Misconfiguration on {{device_hostname}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1649|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|


