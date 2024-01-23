# [Rules](README.md): CVE-2021-44228 Log4j2 Java Library 0-Day Attempt

## Description
Apache Log4j2 <=2.14.1 using JNDI features has an exploit allowing attackers to perform unauthenticated, remote code execution on a Java application that logs user input. This CSE rule looks for attackers attempting to input the string "jndi:" into a field that the application may log to trigger the payload download and execution. This does NOT indicate the application is vulnerable and downloaded the malicious payload, but it does show a hostile actor attempting the attack method.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname, device_ip, srcDevice_ip, srcDevice_hostname, user_username|
|Signal Name|CVE-2021-44228 Log4j2 Java Library 0-Day Attempt|
|Summary Expression|The string "jndi:" was detected inside a CSE field that could be used to attempt CVE-2021-44228.|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|True|
|Tags|_mitreAttackTactic:TA0043, _mitreAttackTechnique:T1595, _mitreAttackTechnique:T1595.001, _mitreAttackTechnique:T1595.002, _mitreAttackTechnique:T1189, _mitreAttackTechnique:T1190, _mitreAttackTechnique:T1133|
## Vendors and Products
- [Akamai - SIEM](../products/9a28f2af-5526-414d-973b-c3fc7984b8a1.md)
- [Akamai - Web Application Firewall](../products/ae07663e-2c2c-4932-be5d-c9f985e95276.md)
- [Amazon AWS - API Gateway](../products/9f76f1fd-fbb0-42d2-9bf5-0f4fd2c1ab82.md)
- [Amazon AWS - Application Load Balancer](../products/5bb9e0b3-8d57-4b10-8952-0b6ffe91b599.md)
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)
- [Amazon AWS - Elastic Load Balancer](../products/59a3cd41-b6d2-4ab7-a0ff-6d5abd14ac43.md)
- [Amazon AWS - Network Firewall](../products/3a82061c-2ca3-4289-9c9b-78756001aa38.md)
- [Amazon AWS - Web Application Firewall (WAF)](../products/072b85a2-1765-45c2-911d-b0509880326e.md)
- [Atlassian - Jira](../products/64088efc-3f28-448d-b386-000deebc7d89.md)
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)
- [Cisco Systems - ASA](../products/be4f7473-fe69-4311-8859-3561900060bf.md)
- [Cisco Systems - Firepower](../products/da9e05a5-3fd3-46a7-a107-ae03c01e3f5a.md)
- [Cisco Systems - Meraki](../products/724c9add-8cd9-4013-b9e1-a907b96da426.md)
- [Cloudflare - Logpush](../products/c2503fcc-ef30-4e40-bb32-0bf47151b140.md)
- [Fortinet - Fortigate](../products/c57e2c85-4fc1-4fb7-8fa1-dbc5235231ad.md)
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)
- [Imperva - Imperva Incapsula](../products/2a236ab1-77d2-4867-a571-a1cfd64528e6.md)
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - IIS](../products/fca8785d-4823-4442-86b2-8acbaa176da4.md)
- [OISF - Suricata IDS](../products/afabb29d-e728-410f-b7c6-acfa9efbe1ed.md)
- [Okta - Single Sign-On](../products/51278354-d6b5-4c8e-a8fd-8197df334e67.md)
- [Palo Alto Networks - Next Generation Firewall](../products/46f5fa2c-1a62-4692-82ad-ed87800a0adb.md)
- [Signal Sciences - Web Application Firewall](../products/2f2fbe08-ab8b-4626-81fd-eaa41b563c49.md)
- [Sophos - UTM 9](../products/0fb003bc-8383-442f-8f3d-afcfbaefe617.md)
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|http_hostname|
|Normalized Schema|http_referer|
|Normalized Schema|http_url|
|Normalized Schema|http_userAgent|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


