# [Rules](README.md): Potential Docker container escape via Cgroups

## Description
A Docker container running with the privileged flag may be exploited by threat actors, potentially resulting in an escape from the Docker container to the host that it is running on. This can result in various privilege escalation opportunities.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname|
|Signal Name|Potential Docker container escape via Cgroups|
|Summary Expression|Potential Docker container escape detected on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1611|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|


