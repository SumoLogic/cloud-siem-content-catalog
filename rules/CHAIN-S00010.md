# [Rules](README.md): Service Installation Followed By Elevated CMD Prompt

## Description
This rule looks for the installation of an application by a non-Sytem user quickly followed by the execution of cmd.exe with System privileges on the same host. This indicates a privilege escalation attempt was likely successful and correlates directly to CVE-2021-41379. The rule is designed to work with standard Security and System event logging, but Sysmon process logging can substitute in place of event ID 4688.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname|
|Signal Name|Service Installation Followed By Elevated CMD Prompt|
|Summary Expression|A possible privilege escalation attempt via service installation was detected on host {{device_hostname}}|
|Score/Severity|Static: 10|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1548, _mitreAttackTechnique:T1548.002|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Direct from Record|fields['EventData.IntegrityLevel']|
|Direct from Record|fields['EventData.MandatoryLabel']|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|parentBaseImage|
|Normalized Schema|parentCommandLine|
|Normalized Schema|user_userId|


