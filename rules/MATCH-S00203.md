# [Rules](README.md): HTTP activity over port 53 - Possible SIGRED

## Description
Detects a possible exploitation of CVE-2020-1350 (aka SIGRED) using rare HTTP requests over port 53. HTTP should rarely (if ever) hosted on port 53. Technique:  T1068.  Derived from SOC Prime logic.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|HTTP activity over port 53 - Possible SIGRED|
|Summary Expression|Possible SIGRED HTTP request to port 53 from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0011, _mitreAttackTechnique:T1071, _mitreAttackTechnique:T1071.001, _mitreAttackTechnique:T1071.004|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [CheckPoint - URL Filtering](../products/2a678bcd-898e-43cd-ab3f-91feb0602a18.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstPort|
|Normalized Schema|http_method|
|Normalized Schema|srcDevice_ip|


