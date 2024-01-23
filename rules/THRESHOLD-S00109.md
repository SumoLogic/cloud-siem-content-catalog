# [Rules](README.md): Azure - Excessive Key Vault Get Requests

## Description
Detects get requests against Vaults, Secrets, and Keys of 25 or greater in a 24 hour period. This may indicate credential access.

 Certain AppId's may need to be excluded if they are expected to be regularly making these requests. Azure Resource Graph's AppId is excluded already.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Credential Access|
|Apply Risk to Entities|device_ip, user_username|
|Signal Name|Azure - Excessive Key Vault Get Requests|
|Summary Expression|Excessive Azure Key Vault Get operations detected from user: {{user_username}} with IP: {{device_ip}} in a 24 hour period.|
|Threshold Count|25|
|Threshold Window|24h|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1526, _mitreAttackTechnique:T1003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|device_ip|
|Direct from Record|fields['identity.claims.appid']|
|Direct from Record|fields['properties.httpStatusCode']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|success|
|Normalized Schema|user_username|


