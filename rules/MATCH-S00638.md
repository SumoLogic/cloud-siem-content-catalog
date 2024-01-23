# [Rules](README.md): McAfee Web Gateway - Suspicious or Malicious Categories

## Description
This rule triggers any time there is a Suspicious or Malicious McAfee Web Gateway category which could indicate there is a problem with the host making the connection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|McAfee Web Gateway - Suspicious or Malicious Categories|
|Summary Expression|Web traffic with category {{http_category}} was found for URL: {{http_url}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_category|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


