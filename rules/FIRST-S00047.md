# [Rules](README.md): First Seen ASN Associated with User for a Successful Azure AD Sign In Event

## Description
This rule will trigger when a new ASN value is associated with a successful Entra ID sign in event for a particular username since the baseline period. This may be suspicious activity as a users IP address may change periodically, but typically users authenticate from a set of ASNs (one ASN value for their home network, another ASN value for their mobile device ) – a sign in with a new ASN not seen since the baseline period could be indicative of credential theft. Look at other events occurring for the user in question for the same time period to ascertain whether access was malicious or benign.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen ASN Associated with User for a Successful Azure AD Sign In Event|
|Summary Expression|{{user_username}} has sucessfully signed into an Azure resource with a first seen ASN of {{device_ip_asnOrg}} since the baseline period.|
|Retention Window|7776000000|
|Baseline Window|5184000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|errorCode|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|objectType|
|Normalized Schema|success|
|Normalized Schema|user_username|


