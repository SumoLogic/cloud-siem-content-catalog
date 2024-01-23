# [Rules](README.md): AWS CloudTrail - Root Console Successful Login Observed

## Description
This signal detects when a successful root account login occurred within an AWS account. This privileged account should seldomly be used within an AWS cloud environment. Amazon's best practices state you should only use the root account to create the initial local IAM users and assigned one of the accounts administrative privileges or to perform rare tasks only available to the root user. The security operations center should be aware when the AWS root account is accessed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Root Console Successful Login Observed from {{srcDevice_ip}}|
|Summary Expression|User: {{user_username}} successfully logged on a root|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1078.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['userIdentity.type']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


