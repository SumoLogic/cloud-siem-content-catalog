# [Rules](README.md): AWS WAF Service Tampering

## Description
Detects various AWS WAF API actions that involve the deletion of a WAF service.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_ip, user_username, srcDevice_ip, device_hostname, srcDevice_hostname|
|Signal Name|AWS WAF Service Tampering - {{action}}|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Dynamic: 2 or 3 or 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1562, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562.008, _mitreAttackTechnique:T1562.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Dynamic Signal Score/Severity Translation

The default score of `2` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|DeleteFirewallManagerRuleGroups|5|
|action|DeleteIPSet|3|
|action|DeleteLoggingConfiguration|5|
|action|DeleteRuleGroup|2|
|action|DeleteWebACL|2|
|action|DeleteRule|2|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


