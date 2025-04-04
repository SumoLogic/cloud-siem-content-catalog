# [Rules](README.md): Threat Intel - Destination IP Address (Medium Confidence)

## Description
This rule detects traffic to IP address with a medium confidence rating from a threat intelligence feed.
Note that this rule is disabled by default due to a high likelihood of excessive signal volume and risk assignment to entities triggering this rule as-is. Tuning to reduce signal volume and potential false positives is highly recommended before activating this rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_ip, dstDevice_ip, device_ip, srcDevice_ip, srcDevice_hostname, srcDevice_hostname, dstDevice_hostname, device_hostname, user_username|
|Signal Name|Threat Intel - Medium Confidence Threat Intel Match on Destination IP Address|
|Summary Expression|The record contains a matching destination IP address from a threat intelligence feed: {{dstDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags||
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|type|
|Normalized Schema|user_username|


