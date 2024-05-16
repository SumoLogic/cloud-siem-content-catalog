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
|Summary Expression|{{commandLine}} executed on host: {{device_hostname}} by user: {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1569, _mitreAttackTechnique:T1569.002|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Cylance - Protect](../products/60829f4a-7acb-47d1-ad23-8424fcf83dcb.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


