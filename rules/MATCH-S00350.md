# [Rules](README.md): Suspicious Typical Malware Back Connect Ports

## Description
Detects programs that connect to typical malware back connect ports based on statistical analysis from two different sandbox system databases.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Suspicious Typical Malware Back Connect Ports|
|Summary Expression|Malware back port connection detected from IP: {{srcDevice_ip}} to IP: {{dstDevice_ip}} on port: {{dstPort}} |
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1571|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Direct from Record|fields['EventData.Initiated']|
|Direct from Record|fields['insertionstrings_f08']|
|Normalized Schema|file_path|
|Normalized Schema|listMatches|
|Normalized Schema|lower|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


