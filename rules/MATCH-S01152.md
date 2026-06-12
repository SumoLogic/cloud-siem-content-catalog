# [Rules](README.md): OpenClaw - Skill Installed Out-of-Band

## Description
Detection:
This rule triggers when a file matching *.openclaw*skills*.md is created by a process whose base image is not "node" (the standard OpenClaw runtime). It monitors Sysmon FileCreate events and flags skill file writes that occur outside the official openclaw or clawhub installer processes.

Scenario:
OpenClaw loads skill configuration files from its skills directory to extend its capabilities. An adversary with filesystem access could plant malicious skill files out-of-band — using any process other than node — to establish persistence, having OpenClaw execute attacker-controlled logic whenever a matching query is processed without triggering standard installation monitoring.

Recommended Actions:
Investigate device_hostname and baseImage to identify what process created the skill file, then inspect changeTarget to determine which skill was installed and review its contents for malicious instructions. Verify whether the write was authorized by the system owner.

Tuning Recommendations:
Create match list 'authorized_openclaw_skill_writers' for any legitimate processes that write skill files outside of node (e.g., configuration management or backup agents).

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|OpenClaw skill installed out-of-band on {{device_hostname}}|
|Summary Expression|Out-of-band OpenClaw skill installation detected on {{device_hostname}} by user {{user_username}}  via process {{baseImage}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1546|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedResource|
|Normalized Schema|user_username|


