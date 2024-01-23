# [Rules](README.md): Spike in Failed Share Access by User

## Description
When attempting to pivot within an internal AD network, attacks will attempt to discover and traverse the available network shares. This detects excessive failed share access attempts for the same username based on a daily outlier standard deviation using a designated historic baseline. The minimum floor of failures expected by default is set to 10.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in Failed Share Access by User|
|Summary Expression|Excessive count of failed share access events identified for user: {{user_username}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|1296000000|
|Standard Deviation Threshold|3|
|Floor Value|10|
|Score/Severity|Static: 2|
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


