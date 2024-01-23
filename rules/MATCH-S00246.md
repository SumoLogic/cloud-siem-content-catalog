# [Rules](README.md): AWS CloudTrail - GetSecretValue from non Amazon IP

## Description
The secrets manager service is commonly used by cloud components to retrieve secrets (connection strings etc) while performing routine functions.  This signal identifies when secret values are retrieved via the GetSecretValue API call and the source host does not belong in an Amazon instance IP space.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - GetSecretValue from non Amazon IP|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552, _mitreAttackTechnique:T1552.004, _mitreAttackTechnique:T1552.005|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|device_ip_asnOrg|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_location|
|Normalized Schema|user_username|


