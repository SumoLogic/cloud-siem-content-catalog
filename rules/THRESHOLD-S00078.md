# [Rules](README.md): High Volume of DNS 'Any' Queries

## Description
Observes for a large number of DNS 'Any' queries which may be indicative of a Distributed Denial of Service Attack (DDoS)

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Execution|
|Apply Risk to Entities|dstDevice_hostname, srcDevice_ip, dstDevice_ip|
|Signal Name|High Volume of DNS 'Any' Queries|
|Summary Expression|Large number of DNS 'Any' queries to host : {{dstDevice_hostname}}|
|Threshold Count|200|
|Threshold Window|60m|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1568, _mitreAttackTechnique:T1568.001, _mitreAttackTechnique:T1568.002, _mitreAttackTechnique:T1568.003|
## Vendors and Products
- [Amazon AWS - Route53](../products/e2393771-bda2-414a-8661-0a57069287ad.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Infoblox - Network Identity Operating System](../products/43808f4c-15e9-480c-ab1a-38bdef3b6798.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_queryType|
|Normalized Schema|dstDevice_hostname|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|objectType|
|Normalized Schema|srcDevice_ip|


