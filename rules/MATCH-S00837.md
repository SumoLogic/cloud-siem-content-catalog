# [Rules](README.md): Kubernetes Secrets Enumeration via Kubectl

## Description
Adversaries may enumerate various Kubernetes secrets on hosts they have compromised in order to escalate privileges or to look for persistence avenues.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Discovery|
|Apply Risk to Entities|user_username|
|Signal Name|Kubernetes Secrets Enumeration via Kubectl|
|Summary Expression|Kubectl was used to read Kubernetes secrets on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1613|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Falco - Falco](../products/d6cb76d3-939e-4e02-b399-b15e0278c877.md)
- [Jamf - Jamf](../products/5c2cc0de-ca31-4ef0-bcfa-133fc8b387ad.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|user_username|


