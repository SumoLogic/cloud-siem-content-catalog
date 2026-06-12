# [Rules](README.md): OpenClaw - Shell Launch by Gateway

## Description
Detection:
This rule triggers when a Node.js process with 'openclaw' in its command line spawns shell interpreters such bash, zsh, sh, PowerShell or python. It monitors process creation events to identify when OpenClaw's shell integration features actively execute system commands. Command lines associated with ip neighbor discovery are excluded as these can be a normal part of OpenClaw operation.

Scenario:
OpenClaw's shell integration allows executing system commands, creating elevated risk compared to passive code generation. Shell spawning indicates active execution features being used, potentially exfiltrating source code, accessing sensitive files, or modifying configurations. Best practice configuration suggests all agent processes run in a  sandbox.

Recommended Actions:
Review device_hostname to identify the user, check parentCommandLine to understand the OpenClaw command, and examine baseImage for the shell type. Check endpoint logs for executed commands (file access, network connections, scripts), then if unauthorized, terminate OpenClaw and review what commands were executed. Review whether OpenClaw is configured such that agent processes are run in a sandbox: https://docs.openclaw.ai/gateway/sandboxing

Tuning Recommendations:
Exclude command lines for legitimate shell use by the OpenClaw gateway process.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|OpenClaw Gateway process on {{device_hostname}} launched a shell|
|Summary Expression|OpenClaw process on {{device_hostname}} launched shell {{baseImage}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|user_username|


