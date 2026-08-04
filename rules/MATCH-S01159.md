# [Rules](README.md): Normalized Runtime Detection

## Description
Passes through a container, cloud-native, or application runtime detection (e.g. Falco, Sysdig, Twistlock, Aqua, Contrast ADR) and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_k8s_normalizedPodName, device_k8s_normalizedDeploymentName, device_k8s_normalizedReplicaSetName, baseImage, user_username, srcDevice_ip, device_ip, http_url, application|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Runtime detection: {{threat_signalName}} on {{device_hostname}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products
- [Aqua - Aqua](../products/4c2a186d-6aa5-47da-a6af-7fddfe16b528.md)
- [Contrast Security - Contrast ADR](../products/fa3c148a-4272-4a94-aea2-499ab90424c2.md)
- [Falco - Falco](../products/d6cb76d3-939e-4e02-b399-b15e0278c877.md)
- [Sysdig - Sysdig](../products/55ec1d4a-6985-4f04-8de5-f9812871fda2.md)
- [Twistlock - Twistlock](../products/581D3DD8-4DA7-4192-9E49-320D7AFB8B53.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|application|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|device_k8s_normalizedDeploymentName|
|Normalized Schema|device_k8s_normalizedPodName|
|Normalized Schema|device_k8s_normalizedReplicaSetName|
|Normalized Schema|http_url|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_username|


