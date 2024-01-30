# [Rules](README.md): First Seen HTTP Connection to High Entropy Domain

## Description
A First Seen connection to a domain with high entropy has been observed. Entropy is a measure of randomness, DGA domains used by malware (i.e. g46mbrrzpfszonuk) often have high entropy. Recommended actions are inspect the web traffic from the host to identify possible malicious activity, as well as investigate information on the domain for signs of suspicious acitivty, blacklists, etc.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Exfiltration|
|Apply Risk to Entities|user_username, device_hostname, srcDevice_ip|
|Signal Name|First Seen HTTP Connection to High Entropy Domain {{http_url_fqdn}}|
|Summary Expression|A First Seen Connection to the High Entropy Domain {{http_url_fqdn}} has been observed from {{srcDevice_ip}} by User: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|0|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1567, _mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1568.002, _mitreAttackTactic:TA0010, _mitreAttackTactic:TA0011|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|http_url_entropyFqdn|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|listMatches|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


