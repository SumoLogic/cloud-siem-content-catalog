# [Rules](README.md): SharePoint Server ToolShell Exploitation (CVE-2025-53770, CVE-2025-53771)

## Description
Context:
Exploits against two vulnerabilities in Microsoft SharePoint server, CVE-2025-53770 and CVE-2025-53771, are combined to execute code on Microsoft SharePoint without authentication. This attack has been nicknamed "ToolShell".

Detection:
This detection will trigger on the inital access and uploading of a malicious payload to the vulnerable SharePoint server.

Recommended Actions:
Follow the Microsoft guidance for how to protect against and remediate this attack: https://msrc.microsoft.com/blog/2025/07/customer-guidance-for-sharepoint-vulnerability-cve-2025-53770/#how-to-protect-your-environment

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|device_ip|
|Signal Name|SharePoint Server ToolShell Exploitation on {{device_ip}}|
|Summary Expression|SharePoint vulnerabilities CVE-2025-53770 and CVE-2025-53771 exploited on {{device_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1190|
## Vendors and Products
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_response_statusCode|


