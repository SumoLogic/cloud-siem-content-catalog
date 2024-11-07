# [Rules](README.md): Okta - First Seen Client ID/ASN combo in successful OIDC token grant

## Description
This signal looks for a new Client ID value ( mapped to the user_username field ) and ASN combination being issued an OIDC token, excluding the Okta Browser Plugin and Okta Dashboard. Use the Okta admin portal and look at the "Applications" section to cross-reference the Client ID value - ensure that the IP address that is requesting the token is known and that this operation is expected and authorized.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Okta - First Seen Client ID/ASN combo in successful OIDC token grant for{{user_username}} from ASN {{srcDevice_ip_asnNumber}}|
|Summary Expression|Okta - First Seen Client ID in successful OIDC token grant for Client ID:{{user_username}} from {{device_ip}}|
|Retention Window|3024000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['actor.displayName']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip_asnNumber|
|Normalized Schema|success|
|Normalized Schema|user_username|


