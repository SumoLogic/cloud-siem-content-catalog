# [Rules](README.md): Detect Psexec With Accepteula Flag

## Description
This rule looks for events where PsExec.exe is run with the accepteula flag in the command line. PsExec is a built-in Windows utility that enables you to execute processes on other systems. It is fully interactive for console applications. This tool is widely used for launching interactive command prompts on remote systems. Threat actors leverage this extensively for executing code on compromised systems. If an attacker is running PsExec for the first time, they will be prompted to accept the end-user license agreement (EULA), which can be passed as the argument accepteula within the command line.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Detect Psexec With Accepteula Flag|
|Summary Expression|PSExec has been executed on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1569.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


