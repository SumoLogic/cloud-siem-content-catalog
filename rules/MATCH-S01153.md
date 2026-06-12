# [Rules](README.md): AF_ALG Socket Opened by Unprivileged Process

## Description
Detection:
A unprivileged process on a Linux host opened a socket using the kernel cryptographic API subsystem, 

Scenario:
An unprivileged local user may be attempting to exploit CVE-2026-31431 (CopyFail), a high-severity Linux kernel vulnerability in the cryptographic subsystem that enables root access on affected systems.

Requirements:
This rule is specific to Laurel Linux Audit logs.

Recommended Actions:
Review the process and user to determine whether this activity is a legitimate use of the kernel cryptographic API. if not, investigate any follow-on commands or processes that may indicate successful privilege escalation.

Tuning Recommendations:
If known-legitimate applications in your environment use the kernel cryptographic API, add their process paths to a match list and exclude them using the baseImage field.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username|
|Signal Name|AF_ALG Socket Opened by {{user_username}}|
|Summary Expression|User {{user_username}}  opened an AF_ALG socket via process {{baseImage}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Laurel - Laurel Linux Audit](../products/f3803323-e4d1-4098-96c6-12e5bf2ab1f5.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['SYSCALL.ARGV.1']|
|Direct from Record|fields['SYSCALL.auid']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


