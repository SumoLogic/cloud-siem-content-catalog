# [Rules](README.md): First Seen DNS Request for High Entropy Domain

## Description
A First Seen connection to a domain with high entropy has been observed. Entropy is a measure of randomness, DGA domains used by malware (i.e. g46mbrrzpfszonuk) often have high entropy. Recommended actions are inspect the web traffic from the host to identify possible malicious activity, as well as investigate information on the domain for signs of suspicious acitivty, blacklists, etc.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Exfiltration|
|Apply Risk to Entities|user_username, device_hostname, srcDevice_ip|
|Signal Name|First Seen DNS Request for High Entropy Domain {{dns_queryDomain}}|
|Summary Expression|A First Seen Connection DNS Request for the High Entropy Domain   has been observed: {{dns_queryDomain}} from {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1071.004, _mitreAttackTechnique:T1567, _mitreAttackTechnique:T1102, _mitreAttackTechnique:T1568.002, _mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|dns_queryDomain|
|Normalized Schema|dns_queryDomain_entropyFqdn|
|Normalized Schema|dns_queryDomain_rootDomain|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


