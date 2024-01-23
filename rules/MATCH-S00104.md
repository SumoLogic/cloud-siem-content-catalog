# [Rules](README.md): AWS CloudTrail - IAM Privileged Policy Applied to Role

## Description
This rule identifies both 'attach' and 'put' actions with this privileged policy.  The difference between 'attach' and 'put' is that 'attach' actions apply a managed policy to an item, where a 'put' action indicates the policy is defined in-line and is part of the items definition. Applying privileged policies to items could indicate hostile action that attempts to increase the privilege level of a user or set of users.  There are legitimate times when this will occur, consider this signal in context of other activities that may indicate suspicious behavior.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - IAM Privileged Policy Applied to Role {{fields['requestParameters.roleName']}}|
|Summary Expression|Privileged Policy: [{{fields['requestParameters.policyArn']}}] an Amazon default policy that carries a high level of access was noticed being applied to the role {{fields['requestParameters.roleName']}}|
|Score/Severity|Dynamic: 2 or 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.004|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Dynamic Signal Score/Severity Translation

The default score of `2` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|AttachRolePolicy|2|
|action|PutRolePolicy|3|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['requestParameters.policyArn']|
|Direct from Record|fields['requestParameters.roleName']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


