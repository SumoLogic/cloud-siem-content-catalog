# [Rules](README.md): Potential AWS Security Credential Access via curl

## Description
A curl command being issued to access sensitive AWS actions related to AWS Secret Manager, System Manager, Lambda Functions or RDS should be uncommon and could be an indication of unexpected credential access. Especially if no authorized uses of curl is used to manage AWS systems.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Potential AWS Security Credential Access via curl|
|Summary Expression|Potential AWS Security Credential Access based on the action: {{action}}  via curl {{http_userAgent}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


