# [Rules](README.md): DNS DGA Lookup Behavior - NXDOMAIN Responses

## Description
Adversaries may make use of Domain Generation Algorithms (DGAs) to dynamically identify a destination for command and control traffic rather than relying on a list of static IP addresses or domains. This has the advantage of making it much harder for defenders to block, track, or take over the command and control channel, as there could potentially be thousands of domains that malware can check for instructions. This technique is described in https://attack.mitre.org/techniques/T1483/.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Command and Control|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|DNS DGA Lookup Behavior - NXDOMAIN Responses|
|Summary Expression|Possible DGA domains|
|Threshold Count|300|
|Threshold Window|10m|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.002|
## Vendors and Products
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Cisco Systems - Umbrella](../products/5ba50e74-3c05-4ea8-aeaf-5efde588c60f.md)
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_queryType|
|Normalized Schema|dns_returnCode|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|


