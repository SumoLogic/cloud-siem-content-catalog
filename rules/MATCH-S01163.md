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
- [Akamai - Noname API Security](../products/f92126c2-e9fc-43d1-bd1a-be8273db2991.md)
- [CheckPoint - Avanan](../products/b8956e27-b893-4518-85ff-20835710c3cf.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Egnyte - DLP](../products/114420df-d10c-4e88-92e9-0d95102c1a3d.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Microsoft - Graph Security API](../products/ef42eb74-7444-4fee-b231-b4eb1e7c9660.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Mimecast - Mimecast](../products/54B36B3F-A63F-4BA4-9DE4-02DBF69A429F.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Proofpoint - TRAP](../products/16c76d97-46c9-43f6-ba96-77d63085a4cf.md)
- [Thinkst Canary - Thinkst Canary](../products/bff00521-0a45-4237-b853-cf21860f88bd.md)
- [Varonis - DatAdvantage](../products/4d6a3683-4edb-4330-9e9f-b8608cd63981.md)
- [Varonis - Varonis Alert](../products/16b8a51d-47b3-4f22-82d7-f48f197307ca.md)


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


