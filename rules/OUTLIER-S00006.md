# [Rules](README.md): Spike in Data Transferred Outbound by User

## Description
Observes excessive amount of bytes out proxy traffic from a username based on a daily outlier standard deviation using a designated historic baseline. The minimum sum of bytes out expected by default is set to 600000000.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in Data Transferred Outbound by User|
|Summary Expression|Excessive daily total of bytes out identified for user: {{user_username}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|604800000|
|Standard Deviation Threshold|2|
|Floor Value|600000000|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1030|
## Vendors and Products
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)
- [Symantec - Proxy Secure Gateway](../products/991a55cf-8c5a-49ba-ae72-6f64a002bacf.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bytesOut|
|Normalized Schema|isNull|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


