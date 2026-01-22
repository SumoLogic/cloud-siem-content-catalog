# [Rules](README.md): First Seen Successful Authentication From Unexpected Country

## Description
First Seen rule which triggers when there are at least two successful logins from the same user with different country codes indicating possible credential theft. It is recommended to add filtering criteria to the expression to reduce false positives, such as known VPN addresses.(If degradation issues occur it is recommendation implementing tuning around your expected network)

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|First Seen Successful Authentication From Unexpected Country: {{srcDevice_ip_countryCode}} for User: {{user_username}}|
|Summary Expression|First Seen successful authentication From unexpected country for user: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0006, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTechnique:T1078.004, _mitreAttackTechnique:T1586, _mitreAttackTechnique:T1586.001, _mitreAttackTechnique:T1586.002|
## Vendors and Products
- [Alibaba - ActionTrail](../products/79055042-52c8-4998-b201-bd2cd2dbca1f.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Asana - Asana Audit](../products/7465af5e-516d-40dc-9535-9b463de0660d.md)
- [Atlassian - Atlassian Audit Events](../products/23342262-740c-41b7-9b77-08267ae01612.md)
- [Auth0 - Auth0](../products/0b45ccba-20b4-41e4-973d-b50fd291944d.md)
- [Box - Box](../products/0472f22e-e3fa-4c9f-a529-8355f671927e.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Identity Services Engine](../products/153794da-09e8-48fe-b511-1306fbb94d07.md)
- [Cisco Systems - Router and Switch IOS](../products/1abefd5b-ec3d-49c1-8a54-7e6363d52db0.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [Cyber-Ark - CyberArk Audit](../products/54f01856-e973-4d7b-a3eb-95cc08ff44f5.md)
- [Dropbox - Dropbox](../products/5bfda3d2-03e7-4d9a-8072-c59430a131d7.md)
- [Duo Security - Multi-Factor Authentication (MFA)](../products/acb7e80e-2b66-496c-ba2e-1e7c3933a98e.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Workspace](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [HP - Aruba ClearPass](../products/12aba181-2b31-472c-a685-2be492f4778d.md)
- [JFrog - Artifactory](../products/abe4975e-de65-4f82-8b35-e6ce392e165c.md)
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
- [Palo Alto Networks - GlobalProtect](../products/b0fe0dde-4e19-4712-957b-1ea7418c132e.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [PingIdentity - PingFederate](../products/b0a0ae6d-dd5b-450c-9d68-36d6c61c67b0.md)
- [SailPoint - SailPoint](../products/c3954250-68a0-49c3-ab6a-ef0daa95ff90.md)
- [Slack - Slack](../products/79da6240-7617-49c8-b130-96278579766e.md)
- [Snowflake - Snowflake](../products/8276b520-fdeb-4f79-9f5d-67865818562b.md)
- [VMware - ESXi](../products/8151e52c-df0d-42d2-978f-2d17e24ae41c.md)
- [Workday - Workday](../products/0438df6b-16ba-4da7-a7a7-626316d0061f.md)
- [Zendesk - Zendesk](../products/a301559a-8110-4dd0-a41d-35b9baa1c740.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|normalizedAction|
|Normalized Schema|srcDevice_ip_countryCode|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|
|Normalized Schema|user_username|


