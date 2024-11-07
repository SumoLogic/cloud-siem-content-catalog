# [Rules](README.md): First Seen gpresult execution on host

## Description
This detection is first observed execution of gpresult on a host, this command may be used by attackers to access detailed password policy information in an enterprise environment. Vulnerability scanners and automated processes may trigger this detection, it is recommended to identify and filter these processes out using a Tuning Expression for the corresponding baseImage. On detection, investigating the host and process executing the command to assist in understanding the context of the execution.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Discovery|
|Apply Risk to Entities|device_hostname, device_ip, user_username|
|Signal Name|First Seen gpresult execution on Host:{{device_hostname}}|
|Summary Expression|First Seen gpresult on host: {{device_hostname}} by User: {{user_username}}|
|Retention Window|7776000000|
|Baseline Window|3024000000|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0007, _mitreAttackTechnique:T1201|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|commandLine|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|user_username|

