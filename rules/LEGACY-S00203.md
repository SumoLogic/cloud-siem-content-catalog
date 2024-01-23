# [Rules](README.md): Cisco Umbrella - Proxy Logs with Cisco AMP Detections

## Description
Cisco Umbrella proxy logs with a Cisco AMP disposition of malicious was detected.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Persistence|
|Apply Risk to Entities|srcDevice_ip, dstDevice_natIp, user_username, srcDevice_hostname|
|Signal Name|Cisco Umbrella - Proxy Logs with Cisco AMP Detections|
|Summary Expression|Cisco Umbrella Categorized as malicious per Cisco AMP disposition the URL: {{http_url}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_natIp|
|Direct from Record|fields['amp_disposition']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


