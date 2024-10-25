# [Rules](README.md): Sharepoint - External IP Downloaded Excessive Documents

## Description
This rule detects when a large number of documents are downloaded in a short timeframe. This behavior may be indicative of programmatic means being used to retrieve all data within the repository.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Collection|
|Apply Risk to Entities|device_ip|
|Signal Name|Sharepoint - External IP Downloaded Excessive Documents|
|Summary Expression|Sharepoint - Excessive Documents Downloaded from {{device_ip}}|
|Threshold Count|20|
|Threshold Window|5m|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1213, _mitreAttackTechnique:T1213.002|
## Vendors and Products
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|device_ip_isInternal|
|Direct from Record|fields['Operation']|
|Normalized Schema|file_basename|
|Normalized Schema|http_userAgent|
|Normalized Schema|lower|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|resource|
|Normalized Schema|user_username|


