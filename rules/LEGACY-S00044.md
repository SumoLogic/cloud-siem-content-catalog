# [Rules](README.md): HTTP Shell Script Download Disguised as a Common Web File

## Description
Attackers who have compromised Unix/Linux machines will sometimes download additional payloads using clear text HTTP where a shell script is downloaded disguised with another file extension. This signal looks for HTTP requests to common web file extensions where the network sensor detected a shell script was returned.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP Shell Script Download Disguised as a Common Web File|
|Summary Expression|Download Shellscript mime type with common file extension from IP: {{srcDevice_ip}} from URL: {{http_url}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1036, _mitreAttackTechnique:T1036.004, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_response_respMimeTypes[0]|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|http_url_path|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|


