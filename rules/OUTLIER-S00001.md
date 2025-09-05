# [Rules](README.md): Spike in Login Failures from a User

## Description
Detects excessive failed login attempts for the same username based on a daily outlier standard deviation for said user. This is designed to catch both slow and quick brute force type attacks using a user specific historic baseline. The minimum floor of failures expected by default is set to 10.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Credential Access|
|Apply Risk to Entities|user_username|
|Signal Name|Spike in Login Failures from a User|
|Summary Expression|Excessive count of failure login events identified for user: {{user_username}} based on daily historic activity|
|Retention Window|7776000000|
|Baseline Window|604800000|
|Standard Deviation Threshold|2|
|Floor Value|10|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - VPN](../products/c49882a3-1b3b-4c21-858a-9fd58b05f715.md)
- [CheckPoint - Firewall and VPN](../products/c3c1a4fc-10cc-4155-8a30-a3bb14fc9f31.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Identity Services Engine](../products/153794da-09e8-48fe-b511-1306fbb94d07.md)
- [Cisco Systems - Router and Switch IOS](../products/1abefd5b-ec3d-49c1-8a54-7e6363d52db0.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [Duo Security - Multi-Factor Authentication (MFA)](../products/acb7e80e-2b66-496c-ba2e-1e7c3933a98e.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [HP - Aruba ClearPass](../products/12aba181-2b31-472c-a685-2be492f4778d.md)
- [JFrog - Artifactory](../products/abe4975e-de65-4f82-8b35-e6ce392e165c.md)
- [JumpCloud - IdP](../products/1ed80351-d779-4f1f-9ddb-b3881f19d487.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [ManageEngine - adauditplus](../products/7205db83-88e8-4074-8288-136a6c493d69.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Graph AD Reporting API](../products/fe5a3e8b-8b6e-44c7-92a8-adfb20df5c75.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [OneLogin - OneLogin Single Sign-On](../products/e43ba0e4-1e3f-40c6-8bca-cb06a656a40b.md)
- [Palo Alto Networks - GlobalProtect](../products/b0fe0dde-4e19-4712-957b-1ea7418c132e.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [PingIdentity - PingFederate](../products/b0a0ae6d-dd5b-450c-9d68-36d6c61c67b0.md)
- [RSA - SecurID Runtime](../products/4809be0f-c6f3-4cbb-b1f6-ae9ae817712e.md)
- [RSA - SecurID SinglePoint](../products/90bba037-f944-480e-89fa-a3b104451af3.md)
- [Tenable - Cloud API](../products/1C384C22-411B-49C0-8029-A7F6C13424B1.md)
- [WatchGuard - Fireware](../products/14aa46d3-0710-44b6-9ce3-0a6b8f36b076.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['resultType']|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedAction|
|Normalized Schema|objectType|
|Normalized Schema|success|
|Normalized Schema|user_username|


