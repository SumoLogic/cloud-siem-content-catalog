# [Rules](README.md): Threat Intel - Successful Authentication from Threat Feed IP

## Description
This rule detects successful authentications from an IP address associated with a known malicious campaign as designated by threat intelligence.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_ip, user_username, dstDevice_ip|
|Signal Name|Threat Intel - Successful Authentication from Threat IP|
|Summary Expression|Successful Authentication from Threat IP: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Identity Services Engine](../products/153794da-09e8-48fe-b511-1306fbb94d07.md)
- [Citrix - ADC](../products/d3606245-76d3-4173-a2fe-832c0e71b0f9.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Cyber-Ark - CyberArk Audit](../products/54f01856-e973-4d7b-a3eb-95cc08ff44f5.md)
- [Duo Security - Multi-Factor Authentication (MFA)](../products/acb7e80e-2b66-496c-ba2e-1e7c3933a98e.md)
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [JFrog - Artifactory](../products/abe4975e-de65-4f82-8b35-e6ce392e165c.md)
- [JumpCloud - IdP](../products/1ed80351-d779-4f1f-9ddb-b3881f19d487.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
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


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|OR|
|Normalized Schema|confidence|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|success|
|Normalized Schema|type|
|Normalized Schema|user_username|


