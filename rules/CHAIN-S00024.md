# [Rules](README.md): RDP Brute Force Login Attempt

## Description
Detection:
This rule correlates a high number of failed authentication attempts with repeated inbound connections over port 3389 (the default RDP port).

Scenario:
An adversary may attempt to discover an account password by using brute force tools against hosts that allow Remote Desktop Protocol (RDP) connections.

Recommended Actions:
Review the destination host and consider whether blocking RDP connections to it from the Internet is appropriate. Review the source IP addresses of the brute force activity and consider blocking it at the firewall. Review the account names that are being used in the brute force attacks and consider forcing password resets for the accounts.

Tuning Recommendations: 
Add the IP addresses of your vulnerability scanners to the "vuln_scanners" list. 
Note that this rule is more likely to trigger when the destination host is a multi-user Terminal Server or if more than one user connects to the host from the same IP address (such as via NAT). Increase the record count that trigger this rule if necessary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip, dstDevice_hostname|
|Signal Name|RDP Brute Force Login Attempt|
|Summary Expression|Attempted brute force attack from IP: {{srcDevice_ip}} to Host:  {{dstDevice_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1110.001, _mitreAttackTechnique:T1110|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Zero Networks - Segment](../products/cf2af9e8-bade-4f28-8bca-b30aa41baec4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|dstPort|
|Normalized Schema|logonType|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedCause|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|


