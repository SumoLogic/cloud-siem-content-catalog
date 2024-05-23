# [Rules](README.md): First Seen Session Token Granted to User from New IP

## Description
Session tokens return a temporary set of credentials that cosnist of an access key ID, a secret and a session token. This alert triggers when a session token is issued for the first time since the baseline period.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen IP AWS Session Token Issued to {{user_username}}|
|Summary Expression|An AWS Session token was issued for the first time since the baseline period to {{user_username}} using the IP address of {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|1814400000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1550.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


