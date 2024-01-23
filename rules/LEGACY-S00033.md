# [Rules](README.md): Executable Downloaded - Content-Type Mismatch

## Description
This rule identifies scenarios where an attacker may have attempted to surreptitiously download an executable file by hiding it behind a different Content-Type, such as image/png. This technique has been observed in samples of Trickbot malware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Executable Downloaded - Content-Type Mismatch|
|Summary Expression|Executable downloaded to host: {{srcDevice_ip}} from URL: {{http_url}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1036.005, _mitreAttackTactic:TA0001, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1566.003, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.001, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_response_headers['CONTENT-TYPE']|
|Normalized Schema|bro_http_response_respMimeTypes[0]|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_url_alexaRank|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


