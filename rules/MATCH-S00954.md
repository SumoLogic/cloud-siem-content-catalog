# [Rules](README.md): GitHub - Copilot Seat Cancelled by GitHub

## Description
Observes for GitHub staff manually revoking copilot access for a user. This action is likely to be rare and may be indicative of a user violating the [acceptable use policy for GitHub](https://docs.github.com/en/site-policy/acceptable-use-policies). This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|targetUser_username|
|Signal Name|GitHub - {{targetUser_username}} Copilot Seat Cancelled By GitHub Staff|
|Summary Expression|{{targetUser_username}} Copilot Seat Cancelled By GitHub Staff for possible misuse.|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|targetUser_username|


