# [Rules](README.md): First Seen External Client to AI Runtime

## Description
Detection: This rule triggers when a new external source IP connects to a local AI inference runtime on a host for the first time after the 14-day baseline period, firing once per novel source IP per host.
Scenario: AI runtimes such as Ollama bind to all network interfaces by default and do not require authentication, leaving them vulnerable to unauthorized access when exposed externally. A previously unseen client connecting to a runtime may indicate unauthorized discovery or a new consumer of an internal AI service.
Recommended Actions: Identify the new client IP and verify the runtime is not inadvertently exposed to the internet. Confirm whether the client is an approved consumer of the AI service.
Tuning Recommendations: To exclude approved AI servers that are expected to receive connections, create a match list of their hostnames under Cloud SIEM > Match Lists, or use an existing list of approved hosts, then go to Cloud SIEM > Rule Tuning, create a tuning expression for this rule, choose to exclude, and enter array_contains(listMatches, '<your_list_name>').

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|device_hostname, srcDevice_ip, user_username|
|Signal Name|First Seen Client {{srcDevice_ip}} to AI Runtime on {{device_hostname}}|
|Summary Expression|First seen external client {{srcDevice_ip}} connecting to AI runtime on {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1190, _mitreAtlasTactic:AML.TA0000, _mitreAtlasTechnique:AML.T0040|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|dstPort|
|Direct from Record|fields['EventData.Initiated']|
|Direct from Record|fields['Initiated']|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


