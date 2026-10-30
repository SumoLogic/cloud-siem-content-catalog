# [Rules](README.md): Sensitive Data Sent to Generative AI Tool - Cross-Vendor

## Description
Detection: This unordered chain rule triggers when a Data Loss Prevention (DLP) finding with no destination URL correlates with a POST, PUT or PATCH request to a Generative AI (GenAI) destination for the same entity within 10 minutes.

Scenario: Employees or automated integrations may send sensitive data to Generative AI (GenAI) tools through chat interfaces, direct API calls, or browser extensions, potentially exposing personally identifiable information (PII), protected health information (PHI), credentials, or proprietary source code outside the organization's control. This represents a data governance risk with regulatory, contractual, and intellectual property consequences, as many GenAI providers may retain or use submitted input for model training.

Recommended Actions: Confirm both events describe the same user session by comparing timestamps, source IP, and user identity, and verify the user matches in both events when several users share an egress IP. Identify the data type from the DLP finding, confirm the GenAI destination, and escalate if sensitive data exposure is confirmed.

Tuning Recommendations: To exclude approved GenAI destinations, create a match list named allowed_ai_domains under Cloud SIEM > Match Lists and add the approved domains; the GenAI stage already excludes records that match it. If your approved domains already live in a list with another name, go to Cloud SIEM > Rule Tuning, create a tuning expression for this rule, choose to exclude, and enter array_contains(listMatches, '<your_list_name>').

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname|
|Signal Name|Sensitive Data Sent to Generative AI Tool - Cross-Vendor|
|Summary Expression|DLP alert correlated with GenAI POST from {{srcDevice_ip}} ({{user_username}}) - cross-vendor chain|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1567|
## Vendors and Products
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['PolicyLocator']|
|Direct from Record|fields['dlp_rule_count']|
|Direct from Record|fields['event.entity.entity_security_result.combined_verdict.dlp']|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|http_url_path|
|Normalized Schema|http_url_rootDomain|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


