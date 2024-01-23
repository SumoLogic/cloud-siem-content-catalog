# [Rules](README.md): McAfee Web Gateway - Poor Reputation

## Description
Observes for sites categorized as having a poor reputation by McAfee Web Gateway

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname, device_ip|
|Signal Name|McAfee Web Gateway - Poor Reputation - {{fields['urlCategories']}}|
|Summary Expression|HTTP connection to the following site with a poor reputation of "{{description}}":

{{fields['urlCategories']}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [McAfee - Web Gateway](../products/003d35b3-3ba8-4e93-8776-e5810b4e243e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|description|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['urlCategories']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


