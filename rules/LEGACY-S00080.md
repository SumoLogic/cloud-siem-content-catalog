# [Rules](README.md): SSH Interesting Hostname Login

## Description
"Interesting hostname" in this context include those that start with dns, ns, smtp, mail, pop, imap, www, and ftp.  Using SSH to hosts that appear to be purposed as servers corresponding to one of these hostnames is considered suspicious.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|SSH Interesting Hostname Login|
|Summary Expression|Suspicious hostname logged into SSH from IP {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0004, _mitreAttackTactic:TA0005, _mitreAttackTactic:TA0008, _mitreAttackTactic:TA0042, _mitreAttackTechnique:T1078, _mitreAttackTechnique:T1078.001, _mitreAttackTechnique:T1078.002, _mitreAttackTechnique:T1078.003, _mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021, _mitreAttackTechnique:T1021.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_name|
|Normalized Schema|user_username|


