# [Rules](README.md): SharePoint Server ToolShell Web Shell Interaction (CVE-2025-53771)

## Description
Context:
Exploits against two vulnerabilities in Microsoft SharePoint server, CVE-2025-53770 and CVE-2025-53771 are combined to execute code on Microsoft SharePoint without authentication. This attack has been nicknamed "ToolShell".

Detection:
This detection will trigger on GET requests occurring to the web shell post-exploitation .

Recommended Actions:
Follow the Microsoft guidance for how to protect against and remediate this attack: https://msrc.microsoft.com/blog/2025/07/customer-guidance-for-sharepoint-vulnerability-cve-2025-53770/#how-to-protect-your-environment

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_ip|
|Signal Name|SharePoint Server ToolShell web shell Interaction from {{srcDevice_ip}}|
|Summary Expression|{{srcDevice_ip}}   was observed interacting with a potential web shell on {{device_ip}} .|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1505.003|
## Vendors and Products
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_ip|
|Normalized Schema|http_method|
|Normalized Schema|http_response_statusCode|
|Normalized Schema|srcDevice_ip|


