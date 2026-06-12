# [Rules](README.md): Unexpected Root Process from Unprivileged Login Session

## Description
Detection:
A user executed a program as root on a Linux host while the originating login session belongs to an unprivileged user, which is inconsistent with legitimate privilege escalation workflows.

Scenario:
An attacker who has obtained local code execution may have exploited a privilege escalation vulnerability such as CVE-2026-31431 (CopyFail) to gain root access, then launched a privileged shell or command to establish a foothold.

Requirements:
Process monitoring must be logged on Linux endpoints for this rule to function.

Recommended Actions:
Investigate the process identified in baseImage and the parent process in parentBaseImage. Review the originating login session  for signs of compromise and check for follow-on persistence mechanisms such as new cron jobs, SSH keys, or modified service definitions.

Tuning Recommendations:
If additional setuid binaries in your environment legitimately produce root processes from unprivileged sessions, add their paths to the exclusion list in the rule expression using the baseImage or parentBaseImage fields.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|Root Process Spawned by Unprivileged User {{user_username}}|
|Summary Expression|Process {{baseImage}} executed as root from unprivileged user {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Laurel - Laurel Linux Audit](../products/f3803323-e4d1-4098-96c6-12e5bf2ab1f5.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedResource|
|Normalized Schema|parentBaseImage|
|Normalized Schema|targetUser_userId|
|Normalized Schema|user_userId|
|Normalized Schema|user_username|


