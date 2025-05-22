# [Rules](README.md): Outlier in Data Transferred into an S3 Bucket by User

## Description
[Disabled by Default] Detects unusual amounts of inbound data transfers to S3 buckets (requires AWS Data events). Verify if the user, role, and IP address associated with this activity are authorized. This rule is disabled by default due to potential alert volume. Before enabling, consider excluding authorized users with regular large transfers via match lists, and adjust floor value and model sensitivity as needed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Outlier in Data Transferred into an S3 Bucket by User|
|Summary Expression|Outlier in Data Transferred into an S3 Bucket by {{user_username}}|
|Retention Window|1209600000|
|Baseline Window|604800000|
|Standard Deviation Threshold|1|
|Floor Value|15173320|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1567.002|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["eventCategory"]|
|Normalized Schema|isBlank|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


