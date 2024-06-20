# [Rules](README.md): MS Office Product Spawning Msdt.exe - CVE-2022-30190

## Description
Monitors for exploitation of CVE-2022-30190 as indicated by a Microsoft Office executable spawning msdt.exe. More information on this vulnerability can be found at the Microsoft Security Response Center: https://msrc-blog.microsoft.com/2022/05/30/guidance-for-cve-2022-30190-microsoft-support-diagnostic-tool-vulnerability/

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username, device_hostname|
|Signal Name|MS Office Product Spawning Msdt.exe - CVE-2022-30190|
|Summary Expression|A Microsoft Office product was observed spawning msdt.exe on host {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1203|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|parentBaseImage|
|Normalized Schema|user_username|


