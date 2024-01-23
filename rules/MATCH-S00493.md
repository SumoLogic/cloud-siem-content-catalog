# [Rules](README.md): Backdoor.SSL.BEACON.[CSBundle Ajax]

## Description
From FireEye Red Team Tool Countermeasures: Network detection rule that looks for specific SSL/TLS certificate metadata attempting to masquerade as a legitimate certificate. The content in this rule is looking for a self-signed certificate which is designated within the Cobalt Strike malleable C2 profile.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Command and Control|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|Backdoor.SSL.BEACON.[CSBundle Ajax]|
|Summary Expression|Suspicious SSL/TLS certificate for {{http_url}} on destination host: {{dstDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1573, _mitreAttackTechnique:T1573.001, _mitreAttackTechnique:T1573.002|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_ssl_issuer|
|Normalized Schema|bro_ssl_subject|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['issuer']|
|Direct from Record|fields['subject']|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


