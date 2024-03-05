# [Rules](README.md): Password Attack

## Description
Detects multiple failed login attempts from a single source with unique usernames over a 24 hour timeframe. This is designed to catch both slow and quick password spray type attacks. The threshold and time frame can be adjusted based on the customer's environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip|
|Signal Name|Password Attack|
|Summary Expression|Password attack from IP: {{srcDevice_ip}} host: {{srcDevice_hostname}}|
|Threshold Count|10|
|Threshold Window|24h|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.001, _mitreAttackTechnique:T1586.002, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1110.003, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - CloudWatch](../products/b57c366d-e6a5-4e61-b950-5686a902bc24.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Identity Services Engine](../products/153794da-09e8-48fe-b511-1306fbb94d07.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [Duo Security - Multi-Factor Authentication (MFA)](../products/acb7e80e-2b66-496c-ba2e-1e7c3933a98e.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [ManageEngine - adauditplus](../products/7205db83-88e8-4074-8288-136a6c493d69.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Graph AD Reporting API](../products/fe5a3e8b-8b6e-44c7-92a8-adfb20df5c75.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [OneLogin - OneLogin Single Sign-On](../products/e43ba0e4-1e3f-40c6-8bca-cb06a656a40b.md)
- [Palo Alto Networks - GlobalProtect](../products/b0fe0dde-4e19-4712-957b-1ea7418c132e.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [RSA - SecurID SinglePoint](../products/90bba037-f944-480e-89fa-a3b104451af3.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['resultType']|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


