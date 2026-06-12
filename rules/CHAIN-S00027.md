# [Rules](README.md): OpenClaw - Outbound Connection from Child Process

## Description
Detection:
This ordered chain rule triggers when a child process of an openclaw-gateway node process is created on a host followed within 5 minutes by an outbound network connection to an external IP from the same process on the same host, grouped by process ID and hostname. Command lines associated with ip neighbor discovery are excluded as these can be a normal part of OpenClaw operation.

Scenario:
OpenClaw's gateway process spawns child processes (shells, scripts) to execute system commands during code intelligence operations. When these child processes establish outbound connections to external IPs, it indicates potential data exfiltration — code, credentials, or other sensitive content being transmitted from the host via OpenClaw's execution capability.

Recommended Actions:
Investigate device_hostname and baseImage to identify the child process and user, then review dstDevice_ip to determine the external destination. Correlate with DNS logs and firewall records to assess what data may have been transmitted, and inspect OpenClaw skill files for injected commands.

Tuning Recommendations:
Create match list 'authorized_openclaw_external_destinations' for known legitimate external IPs contacted by OpenClaw child processes. Adjust the 5-minute correlation window if legitimate use cases show longer delays between process creation and network activity.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Exfiltration|
|Apply Risk to Entities|device_hostname|
|Signal Name|OpenClaw - Outbound Connection from Child Process|
|Summary Expression|OpenClaw gateway child process  made an outbound network connection from host {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1041|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|normalizedAction|
|Normalized Schema|normalizedResource|


