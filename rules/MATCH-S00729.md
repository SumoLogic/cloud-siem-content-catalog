# [Rules](README.md): MacOS Gatekeeper Bypass

## Description
The com.apple.quarantine flag is usually automatically set for downloaded files and invokes Apple's Gatekeeper program for file analysis. As such, attackers may attempt to remove this flag from malware payloads using the xattr command. Note that files downloaded via curl, external media, or from shared drives on the local network do not set the com.apple.quarantine flag.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|device_hostname, user_username, device_ip|
|Signal Name|MacOS Gatekeeper Bypass|
|Summary Expression|User {{user_username}} ran the command "{{commandLine}}" on host {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1553.001, _mitreAttackTactic:TA0005|
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|


