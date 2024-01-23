# [Rules](README.md): vpnoverdns.com DNS lookup

## Description
vpnoverdns.com is a free service providing VPN functionality over DNS. DNS resolutions for *.tun.vpnoverdns.com indicate usage of their VPN service. The service describes itself as "Data exfiltration, for those times when everything else is blocked.".

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Exfiltration|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_hostname, srcDevice_ip, user_username|
|Signal Name|vpnoverdns.com DNS lookup|
|Summary Expression|VPN over DNS from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0010, _mitreAttackTechnique:T1133|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|dns_query|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


