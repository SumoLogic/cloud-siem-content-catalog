# [Rules](README.md): Threat Intel - Source Hostname

## Description
This rule detects an indicator match from a threat intelligence feed

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Threat Intelligence|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, srcDevice_natIp, srcDevice_mac, user_username, dns_replyIp|
|Signal Name|Threat Intel - Source Hostname|
|Summary Expression|Threat Intel - Source Device Hostname detected for: {{srcDevice_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Abnormal Security - Abnormal Security](../products/2b79254e-8017-4dbf-8e39-590132172a7d.md)
- [Infoblox - Network Identity Operating System](../products/43808f4c-15e9-480c-ab1a-38bdef3b6798.md)
- [OpenSSH - sshd](../products/940dba19-cb65-4768-bf97-75bf5433ddd4.md)
- [Proofpoint - Proofpoint on Demand](../products/332856e9-3111-446f-8df7-e64694e4b9a1.md)
- [Zscaler - Nanolog Streaming Service](../products/6299d728-14f7-455e-85c5-ea8ec65a654a.md)
- [Zscaler - ZPA Log Streaming Service](../products/4a75a995-0e10-45fc-8b4d-7fcfc0e98e25.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_replyIp|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_mac|
|Normalized Schema|srcDevice_natIp|
|Normalized Schema|user_username|


