# [Rules](README.md): Sensitive Data Sent to Generative AI Tool

## Description
Detection: This rule triggers when a single record contains both a Data Loss Prevention (DLP) finding and a write request (POST, PUT, PATCH, upload or edit) to a Generative AI (GenAI) destination, identified by domain list or Cloud Access Security Broker category.

Scenario: Employees or automated integrations may send sensitive data to GenAI tools through chat interfaces, direct API calls, or browser extensions, exposing personal data, credentials or source code outside the organization's control. This is a data governance risk, as many GenAI providers may retain or use submitted input for model training.

Recommended Actions: Review the DLP finding details and identify which GenAI tool was used. Determine whether the activity was intentional or accidental, and escalate if credentials, protected health information, or source code are confirmed.

Tuning Recommendations: To exclude approved GenAI destinations, create a match list named allowed_ai_domains under Cloud SIEM > Match Lists, set its target column to Domain, and add the approved domains; this rule already excludes records that match it.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname|
|Signal Name|Sensitive Data Sent to {{http_url_fqdn}}|
|Summary Expression|Sensitive data sent to {{http_url_fqdn}} by {{user_username}} from {{srcDevice_ip}}|
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
|Direct from Record|fields['dlp_rule_count']|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|http_url_rootDomain|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


