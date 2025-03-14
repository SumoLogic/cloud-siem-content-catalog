# [Rules](README.md): Azure DevOps - Known Malicious Tooling Detected ADOKit

## Description
Context:
The IBM X-Force Red team released the Azure DevOps Services Attack Toolkit (ADOKit) for Black Hat Arsenal 2024.

Detection:
This is a simple detection matching on “ADOKit” at the start of the HTTP User Agent String (UAS). This detection effectively catches basic ADOKit use. It is brittle to attackers changing the User Agent String to another more innocuous browser to mask the traffic.

Recommended Actions: 
Determine the user using the ADOKit tooling and the activities they have taken against the Azure DevOps environment.

Tuning Recommendations:
Create a rule tuning expression to tune out accounts permitted to use ADOKit, such as red teams, penetration testers, or admin users. 

Credits:
This detection is based on the Azure Sentinel ADOMaliciousToolingDetections1.yaml detection.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Collection|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|Azure DevOps - ADOKit malicious tooling from IP: {{srcDevice_ip}}|
|Summary Expression|Detected use of malicious tooling ADOKit by User: {{user_username}} from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1119, _mitreAttackTactic:TA0009|
## Vendors and Products
- [Microsoft - Azure DevOps Auditing](../products/c3b61ddb-4d2d-497c-b873-28938036b67b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


