# [Rules](README.md): Normalized Runtime Detection

## Description
Passes through a container or cloud-native runtime detection (e.g. Falco, Sysdig, Twistlock, Aqua) and adjusts the severity accordingly based on the severity provided in the log.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_k8s_normalizedPodName, device_k8s_normalizedDeploymentName, device_k8s_normalizedReplicaSetName, baseImage, user_username|
|Signal Name|{{metadata_vendor}} {{metadata_product}} - {{threat_signalName}}|
|Summary Expression|Runtime detection: {{threat_signalName}} on {{device_hostname}}|
|Score/Severity|None|
|Enabled by Default|True|
|Prototype|False|
|Tags||
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|device_k8s_normalizedDeploymentName|
|Normalized Schema|device_k8s_normalizedPodName|
|Normalized Schema|device_k8s_normalizedReplicaSetName|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|normalizedSeverity|
|Normalized Schema|threat_ruleType|
|Normalized Schema|threat_signalName|
|Normalized Schema|user_username|


