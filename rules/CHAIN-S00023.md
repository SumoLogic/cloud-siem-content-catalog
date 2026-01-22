# [Rules](README.md): Administrative Remote Interactive Brute Force Login

## Description
Detection:
This rule correlates a high number of failed authentication attempts with  a successful remote interactive login (such as via RDP) coming from the same source IP address and user account. 

Context:
An adversary may discover an account password by using brute force tools against hosts that allow Remote Desktop Protocol (RDP) connections. Upon discovering the correct password the attacker proceeds to log in via RDP.

Recommended Actions:
Determine whether this activity was benign, ideally by contacting the user. If the activity is determined to be malicious, log out all sessions from the compromised account and force a password reset. Investigate the activities of the user account originating from the RDP host to look for signs of persistence and lateral movement. Consider taking the RDP host offline for investigation. Block all connections from the source host.

Tuning Recommendations: 
Add the IP addresses of your vulnerability scanners to the "vuln_scanners" list. Adjust the record counts that trigger this rule if necessary.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Unknown/Other|
|Apply Risk to Entities|dstDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Administrative Remote Interactive Brute Force Login|
|Summary Expression|Successful administrative remote interactive brute force login from IP: {{srcDevice_ip}} to Host:  {{dstDevice_hostname}}  from user {{user_username}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1078|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|logonType|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedCause|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|success|
|Normalized Schema|user_username|


