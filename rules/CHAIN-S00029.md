# [Rules](README.md): Suspicious Child Process Spawned After Python Model Deserialization

## Description
Detection: This ordered chain rule triggers when a Python process referencing a serialized model file (.pkl, .pth, .pt, .ckpt, .joblib) or deserialization function (pickle.load, torch.load, joblib.load) in its command line is followed by a child process executing a reverse shell, download-and-execute, credential access, or encoded payload on the same host within 10 minutes.

Scenario: Engineers routinely download and load pretrained models from public repositories. Attackers exploit this by publishing weaponized models that execute arbitrary code during deserialization via Python's __reduce__ method - JFrog researchers identified multiple such models on HuggingFace establishing reverse shells upon loading. Link: https://jfrog.com/blog/data-scientists-targeted-by-malicious-hugging-face-ml-models-with-silent-backdoor/

Recommended Actions: Identify the model file from the Python process command line and confirm the child process activity. Investigate whether the child process PID traces back to the Python process to strengthen attribution, check the model file origin, and isolate the host if malicious activity is confirmed.

Tuning Recommendations: To exclude CI/CD build servers and automation hosts that routinely run Python scripts spawning shell commands, create a match list named ci_cd_hosts of their hostnames under Cloud SIEM > Match Lists; the child-process stage already excludes records that match it, so no further change is needed.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Execution|
|Apply Risk to Entities|device_hostname, user_username, srcDevice_ip|
|Signal Name|Suspicious Child Process Spawned After Python Model Deserialization|
|Summary Expression|Suspicious child process spawned after Python model deserialization on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.006, _mitreAttackTechnique:T1059.004, _mitreAttackTechnique:T1204.002, _mitreAtlasTactic:AML.TA0005, _mitreAtlasTechnique:AML.T0011.000|
## Vendors and Products
- [Linux - Sysmon for Linux](../products/b238758d-ade8-41d2-b32d-c99159e9fd74.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


