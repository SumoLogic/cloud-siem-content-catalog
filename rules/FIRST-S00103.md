# [Rules](README.md): First Seen AI Runtime on Endpoint

## Description
Detection: This rule triggers when an AI inference runtime process appears on a host for the first time after the 14-day baseline period, firing once per novel runtime per host.
Scenario: A previously unseen AI runtime on a corporate endpoint may indicate an unauthorized installation or a new tool adoption that has not been reviewed by IT or security. Early visibility into new runtime deployments supports AI governance programs and shadow IT detection.
Recommended Actions: Investigate why a new AI runtime appeared on this host. Determine whether it was installed by the user or deployed through an approved channel, and verify the host is authorized for AI workloads.
Tuning Recommendations: To exclude approved AI hosts, create a match list of their hostnames under Cloud SIEM > Match Lists, or use an existing list of approved hosts, then go to Cloud SIEM > Rule Tuning, create a tuning expression for this rule, choose to exclude, and enter array_contains(listMatches, '<your_list_name>').

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|First Seen: {{baseImage}} on {{device_hostname}}|
|Summary Expression|AI runtime {{baseImage}} first seen on {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1204.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Osquery - Osquery](../products/93e2d3d-fab1-4d61-845f-49bc1ae5bed9.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|user_username|


