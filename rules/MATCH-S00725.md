# [Rules](README.md): Microsoft CHM File Observed

## Description
Compiled HTML Files (.chm) are blocked by default on modern Windows operating systems and are also vulnerable to malicious code embedding. These factors make the presence of .chm files on company assets both unusual and risky.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, device_hostname, device_ip|
|Signal Name|Microsoft CHM File Observed|
|Summary Expression|A .chm file was observed on host {{device_hostname}} in association with user {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1218.001|
## Vendors and Products
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Code42 - Incydr](../products/cc523ad6-7193-4de5-a254-d0243fca63f3.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Egnyte - DLP](../products/114420df-d10c-4e88-92e9-0d95102c1a3d.md)
- [FireEye - Endpoint Security](../products/8c342fa0-4147-47c9-b574-965ad2eddafa.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [ManageEngine - adauditplus](../products/7205db83-88e8-4074-8288-136a6c493d69.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Netskope - Security Cloud](../products/B3582ED2-1A0C-452D-9802-97433D143486.md)
- [Palo Alto Networks - Cortex XDR](../products/146522A1-DC9A-40A5-A909-2EB3B665B1D1.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


