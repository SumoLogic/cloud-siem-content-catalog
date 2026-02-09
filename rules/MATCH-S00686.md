# [Rules](README.md): Base64 Decode in Command Line

## Description
Malicious files are often encoded in an attempt to bypass security controls that would otherwise inspect the contents of said file. An attacker would then need to decode the malicious file for use on the victim machine using a utility such as certutil or the base64 command. This rule supports detection for standard decoding utilities on Unix, Windows cmd, Windows PowerShell, and MacOS.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Base64 Decode in Command Line|
|Summary Expression|A base64-encoded file was decoded on host {{device_hostname}} by user {{user_username}}|
|Score/Severity|Static: 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1140, _mitreAttackTactic:TA0011, _mitreAttackTechnique:T1132.001, _mitreAttackTechnique:T1132|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [CrowdStrike - Filevantage](../products/a1f79987-b765-4f6f-bfe5-d657baa35144.md)
- [Cyber-Ark - Enterprise Password Vault](../products/36f5ca33-0c1e-4223-8215-977ea04425ba.md)
- [Falco - Falco](../products/d6cb76d3-939e-4e02-b399-b15e0278c877.md)
- [Jamf - Jamf](../products/5c2cc0de-ca31-4ef0-bcfa-133fc8b387ad.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Systemd Journal](../products/5be5af82-c248-4c4c-a485-0571025f242c.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [SentinelOne - SentinelOne](../products/8967aecc-ffb3-4cbe-a02e-258d1edca8d0.md)
- [Sysdig - Sysdig](../products/55ec1d4a-6985-4f04-8de5-f9812871fda2.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


