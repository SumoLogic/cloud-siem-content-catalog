# [Rules](README.md): Threat Intel - Matched File Hash

## Description
A record flagged a file hash from a threat intelligence match list

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|device_hostname, srcDevice_hostname, device_ip, device_natIp, srcDevice_ip, srcDevice_natIp, device_mac, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - Matched File Hash|
|Summary Expression|None|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Bitdefender - GravityZone](../products/046b3623-69fe-409f-9e80-fd3ebef0654f.md)
- [Cisco Systems - Advanced Malware Protection (AMP)](../products/7eaa4c44-5b7f-4d9e-8c1c-c4105c2b7506.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Cyber-Ark - Endpoint Privilege Manager](../products/96d1bd4a-9285-439e-b81c-1a32f7688dac.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Graph Security API](../products/ef42eb74-7444-4fee-b231-b4eb1e7c9660.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Cortex XDR](../products/146522A1-DC9A-40A5-A909-2EB3B665B1D1.md)
- [Proofpoint - Proofpoint on Demand](../products/332856e9-3111-446f-8df7-e64694e4b9a1.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)
- [Sophos - Central](../products/e5a708c9-82be-4df9-8ea0-07cac95abf2a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|device_mac|
|Normalized Schema|device_natIp|
|Normalized Schema|dns_replyIp|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|
|Normalized Schema|srcDevice_natIp|
|Normalized Schema|user_username|


