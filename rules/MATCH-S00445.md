# [Rules](README.md): Known Ransomware File Extensions

## Description
Observes for common file extensions associated with ransomware indicating the presence of encrypted files.

Some known ransomware file extensions are shared with other applications and may cause this rule to fire.

File extension list sourced from:
https://techviral.net/ransomware-encrypted-file-extensions/

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Impact|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Known Ransomware File Extensions|
|Summary Expression|Known ransomware file extention for file: {{file_path}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1486|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Egnyte - DLP](../products/114420df-d10c-4e88-92e9-0d95102c1a3d.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Malwarebytes - Malwarebytes Endpoint Protection](../products/e611250c-6b5f-4b40-b84b-329a1d5b391c.md)
- [ManageEngine - adauditplus](../products/7205db83-88e8-4074-8288-136a6c493d69.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Varonis - DatAdvantage](../products/4d6a3683-4edb-4330-9e9f-b8608cd63981.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


