# [Rules](README.md): Spike in Failed Azure Sign In Attempts Due to Bad Password from IP Address

## Description
Outlier in Failed Azure Sign In Attempts Due to Bad Password from IP Address due to exceeded standard deviation of what is expected for the IP Address based on a historic baseline. The minimum floor of failures expected by default is set to 2.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Credential Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Spike in Failed Azure Sign In Attempts Due to Bad Password from IP Address: {{srcDevice_ip}}|
|Summary Expression|Outlier in count of failures identified from IP Address: {{srcDevice_ip}} based on hourly historic activity|
|Retention Window|7776000000|
|Baseline Window|432000000|
|Standard Deviation Threshold|2|
|Floor Value|2|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110.001|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields["properties.status.errorCode"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


