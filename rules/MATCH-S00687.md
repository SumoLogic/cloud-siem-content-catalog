# [Rules](README.md): Linux Security Tool Usage

## Description
This rule monitors for usage of the default command or script names associated with penetration testing tools used on Linux machines. While these commands can be renamed to avoid detection, less sophisticated attackers will often neglect to do so.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|Linux Security Tool Usage|
|Summary Expression|A Linux security tool was launched on host {{device_hostname}} by user {{user_username}}|
|Score/Severity|Static: 7|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [CrowdStrike - Falcon](../products/840c72e0-4e47-41e7-9b93-31f55d12f07d.md)
- [Cyber-Ark - Enterprise Password Vault](../products/36f5ca33-0c1e-4223-8215-977ea04425ba.md)
- [Jamf - Jamf](../products/5c2cc0de-ca31-4ef0-bcfa-133fc8b387ad.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)
- [Sysdig - Sysdig](../products/55ec1d4a-6985-4f04-8de5-f9812871fda2.md)
- [Trend Micro - Vision One](../products/72a5ddec-abb9-41ff-a2da-6a58beff980c.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|lower|
|Normalized Schema|user_username|


