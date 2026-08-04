# [Rules](README.md): Normalized Data Protection Detection

## Description
Passes through a data-protection, email, or deception detection (e.g. DLP, Proofpoint, Thinkst Canary) and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|resource, file_path, user_email, user_username, srcDevice_ip|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Data protection detection: {{threat_signalName}} on {{resource}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|file_path|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|resource|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_email|
|Normalized Schema|user_username|


