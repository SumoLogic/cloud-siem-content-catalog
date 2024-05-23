# [Rules](README.md): chage command use on host

## Description
The chage command on Linux allows for the changing of user password expiry information. The chage command is restricted to the root user; however, non-root/unprivileged users may use the -l flag to determine when the user’s password or account is due to expire.  It is recommended to investigate the system and account the command has been executed on, to assess the intent of this execution. Additionally, looking at the command line and parent process is helpful in identifying valid automated processes executing this command that would benefit from tuning out via Rule Tuning.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|chage command usage detected on Host:{{device_hostname}}|
|Summary Expression|Cxecution of the chage command has been detected on Host: {{device_hostname}} by User: {{user_username}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


