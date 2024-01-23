# [Rules](README.md): ZScaler Proxy-Traffic to Malicious Categorized Domain

## Description
Observes for traffic detected and categorized as malicious by ZScaler

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|ZScaler Proxy-Traffic to Malicious Categorized Domain|
|Summary Expression|ZScaler Detected Traffic to Malicious Categorized Domain from {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Zscaler - Firewall](../products/9e0641a7-22ce-4ac8-8113-ee48b368ac3d.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['cat']|
|Direct from Record|fields['category']|
|Direct from Record|fields['description']|
|Direct from Record|fields['urlcat']|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


