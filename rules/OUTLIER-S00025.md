# [Rules](README.md): AWS S3 Outlier in PutObject Denied Events

## Description
This rule utilizes an hourly baseline to detect an outlier in the number of denied PutObject access events to an S3 bucket. AWS Data events are necessary for this signal to function. Denied PutObject access events can stem from IAM policies or bucket policies. Look at the user, role, IP address from the events in order to determine whether this activity is expected. In certain cases, access denied events to S3 can also result in unexpected AWS charges.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in AWS S3 PutObject Denied Events|
|Summary Expression|An outlier in AWS S3 PutObject Denied Events was detected for: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|1|
|Floor Value|5|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1567.002|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Direct from Record|fields["errorCode"]|
|Direct from Record|fields["errorMessage"]|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


