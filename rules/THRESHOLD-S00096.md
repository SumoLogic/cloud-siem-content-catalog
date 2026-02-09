# [Rules](README.md): Brute Force Attempt

## Description
Detects multiple failed login attempts for the same username over a 24 hour timeframe. This is designed to catch both slow and quick brute force type attacks. The threshold and time frame can be adjusted based on the customer's environment.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Brute Force Attempt|
|Summary Expression|Multiple failed login attempts for user: {{user_username}}|
|Threshold Count|10|
|Threshold Window|24h|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1586, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1110.002, _mitreAttackTechnique:T1110.001|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Auth0 - Auth0](../products/0b45ccba-20b4-41e4-973d-b50fd291944d.md)
- [Bitwarden - Bitwarden](../products/ebb99eec-3585-4673-ac0f-676632a78305.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Identity Services Engine](../products/153794da-09e8-48fe-b511-1306fbb94d07.md)
- [Cisco Systems - Router and Switch IOS](../products/1abefd5b-ec3d-49c1-8a54-7e6363d52db0.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Dropbox - Dropbox](../products/5bfda3d2-03e7-4d9a-8072-c59430a131d7.md)
- [Duo Security - Multi-Factor Authentication (MFA)](../products/acb7e80e-2b66-496c-ba2e-1e7c3933a98e.md)
- [F5 - F5](../products/ede052db-d472-408f-949c-be642237ef3f.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [HP - Aruba ClearPass](../products/12aba181-2b31-472c-a685-2be492f4778d.md)
- [JumpCloud - Directory Insights](../products/05bfaf47-5e21-4d5f-b724-98960a6fca8a.md)
- [JumpCloud - IdP](../products/1ed80351-d779-4f1f-9ddb-b3881f19d487.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Graph AD Reporting API](../products/fe5a3e8b-8b6e-44c7-92a8-adfb20df5c75.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Mimecast - Mimecast](../products/54B36B3F-A63F-4BA4-9DE4-02DBF69A429F.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [OneLogin - OneLogin Single Sign-On](../products/e43ba0e4-1e3f-40c6-8bca-cb06a656a40b.md)
- [OpenVPN - OpenVPN](../products/9f6d624f-6d8f-43c7-a4b0-51179061631c.md)
- [Palo Alto Networks - GlobalProtect](../products/b0fe0dde-4e19-4712-957b-1ea7418c132e.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [PingIdentity - PingFederate](../products/b0a0ae6d-dd5b-450c-9d68-36d6c61c67b0.md)
- [Pritunl - Pritunl](../products/70f80fa8-200a-449b-8100-f8d4b7687380.md)
- [RSA - SecurID Runtime](../products/4809be0f-c6f3-4cbb-b1f6-ae9ae817712e.md)
- [RSA - SecurID SinglePoint](../products/90bba037-f944-480e-89fa-a3b104451af3.md)
- [Salesforce - Salesforce](../products/1b7798df-963b-4582-a82b-b8176c3a6a22.md)
- [Slack - Slack](../products/79da6240-7617-49c8-b130-96278579766e.md)
- [Snowflake - Snowflake](../products/8276b520-fdeb-4f79-9f5d-67865818562b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields['resultType']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedAction|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


