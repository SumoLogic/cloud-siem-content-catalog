# [Rules](README.md): First Seen User Creating or Modifying EC2 Launch Template

## Description
AWS EC2 launch templates allows cloud administrators to specify instance configuration information in a templated format. Granting permissions to modify or create launch templates within EC2 in certain circumstances grants the user PassRole permissions, potentially opening privilege escalation avenues via IAM. The following AWS documentation outlines this behavior: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/permissions-for-launch-templates.html. Look at other events the user in question is performing in order to investigate this signal. Consider excluding authorized users via a match list if this signal is triggering too many false positives.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen User Creating or Modifying EC2 Launch Template|
|Summary Expression|First Seen User: {{user_username}}  Creating or Modifying EC2 Launch Template|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTactic:TA0004, _mitreAttackTechnique:T1578.002, _mitreAttackTechnique:T1578|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


