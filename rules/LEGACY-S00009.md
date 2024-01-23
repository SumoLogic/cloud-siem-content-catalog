# [Rules](README.md): Bluecoat Proxy - Suspicious or Malicious Categories

## Description
This rule triggers any time there is a Suspicious or Malicious Bluecoat category which could indicate there is a problem with the host making the connection. 

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, user_username, srcDevice_hostname|
|Signal Name|Bluecoat Proxy - Suspicious or Malicious Categories|
|Summary Expression|URL categorized as Suspicious or Malicious by Proxy|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001|
## Vendors and Products
- [Symantec - Proxy Secure Gateway](../products/991a55cf-8c5a-49ba-ae72-6f64a002bacf.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['category']|
|Direct from Record|fields['cs-categories']|
|Direct from Record|fields['device_event_category']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


