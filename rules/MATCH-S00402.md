# [Rules](README.md): Normalized Security Signal

## Description
Passes through an alert from an endpoint security product and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, device_ip, srcDevice_ip, user_username|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Threat: {{threat_name}} detected on host: {{device_hostname}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Amazon AWS - GuardDuty](../products/2ca0adcf-7616-4474-8557-a3773515aa6d.md)
- [Amazon AWS - Security Hub](../products/d0aebc1c-db4d-440f-b69f-70dae24befff.md)
- [Bitdefender - GravityZone](../products/046b3623-69fe-409f-9e80-fd3ebef0654f.md)
- [Carbon Black - Defense](../products/4448ca62-bb4f-4859-a6a2-d9262f9e48f0.md)
- [CheckPoint - Avanan](../products/b8956e27-b893-4518-85ff-20835710c3cf.md)
- [Cisco Systems - Advanced Malware Protection (AMP)](../products/7eaa4c44-5b7f-4d9e-8c1c-c4105c2b7506.md)
- [Claroty - Claroty xDome](../products/8cdfb3fc-8700-4012-bf3d-7dfc147d291b.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Egnyte - DLP](../products/114420df-d10c-4e88-92e9-0d95102c1a3d.md)
- [FireEye - Central Management System](../products/a4b7d3df-ec31-4c94-bf09-2f790db91de1.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - G Suite](../products/e73cd65a-7a4b-4ce9-9d73-e5d9c824c214.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Microsoft - Advanced Threat Analytics](../products/ae48ad1f-04e5-47c6-9892-25555e5f728b.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Graph Identity Protection API](../products/4da7313c-5123-4eae-bb84-5d868fc55a74.md)
- [Microsoft - Graph Security API](../products/ef42eb74-7444-4fee-b231-b4eb1e7c9660.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - Cortex XDR](../products/146522A1-DC9A-40A5-A909-2EB3B665B1D1.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Palo Alto Networks - Prisma Cloud](../products/343b9323-d279-40d9-946f-809242e5cf98.md)
- [Qualys - VMScan](../products/08d5e888-ae62-462a-80d9-c0df7d3643c1.md)
- [Sophos - Central](../products/e5a708c9-82be-4df9-8ea0-07cac95abf2a.md)
- [Trend Micro - Apex Central](../products/F362EA03-9BBB-4701-B2DF-5460C4A289CF.md)
- [Trend Micro - Deep Security](../products/57cec26c-f94e-4403-add4-dae2382b5c16.md)
- [VMware - Carbon Black Cloud](../products/f9cea291-9030-4e41-9836-6dd9274d6df4.md)
- [Varonis - DatAdvantage](../products/4d6a3683-4edb-4330-9e9f-b8608cd63981.md)
- [Varonis - DatAlert](../products/bd98578e-3f97-4e5a-93ec-bbff28f90ccf.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_username|


