# [Rules](README.md): Microsoft Support Diagnostic Tool Invoking PowerShell - CVE-2022-30190

## Description
Monitors for exploitation of CVE-2022-30190 as indicated by the Microsoft Support Diagnostic Tool Invoking PowerShell. More information on this vulnerability can be found at the Microsoft Security Response Center: https://msrc-blog.microsoft.com/2022/05/30/guidance-for-cve-2022-30190-microsoft-support-diagnostic-tool-vulnerability/

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|user_username, device_hostname, device_ip|
|Signal Name|Microsoft Support Diagnostic Tool Invoking PowerShell - CVE-2022-30190|
|Summary Expression|Microsoft Support Diagnostic Tool Invoking PowerShell on host {{device_hostname}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1203|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


