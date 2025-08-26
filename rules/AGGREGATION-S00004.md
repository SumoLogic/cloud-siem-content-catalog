# [Rules](README.md): Suspicious K8s Enumeration

## Description
Threat actors will attempt to enumerate various system settings in order to explore privilege escalation avenues or to locate potentially sensitive data.

## Additional Details
|Detail|Value|
|----|----|
|Type|Aggregation|
|Category|Unknown/Other|
|Apply Risk to Entities|device_hostname|
|Signal Name|Suspicious K8s Enumeration|
|Summary Expression|{{device_hostname}} has recorded a number of Kubernetes enumeration commands issued in rapid succession, indicating a potentially malicious system enumeration attempt.|
|Aggregation Window|T05M|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|True|
|Tags||
## Vendors and Products
- [CrowdStrike - FDR](../products/569a3a44-c29f-492e-bcf4-5dc04e2ab0f3.md)
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cmd_count|
|Normalized Schema|device_hostname|


