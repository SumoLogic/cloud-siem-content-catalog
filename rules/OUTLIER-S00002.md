# [Rules](README.md): Spike in Successful Distinct Share Access

## Description
When attempting to pivot within an internal AD network, attacks will attempt to discover and traverse the available network shares. This detects successful and unique share access attempts for the same username based on a daily outlier standard deviation using a designated historic baseline. The minimum floor of unique shares expected by default is set to 5.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in Successful Share Access|
|Summary Expression|Excessive distinct amount of successful share access events identified for user: {{user_username}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|1|
|Floor Value|5|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1135|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["Keywords"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


