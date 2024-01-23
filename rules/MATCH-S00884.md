# [Rules](README.md): macOS - Suspicious Python PIP Execution

## Description
This alert utilizes Jamf telemetry and looks for suspicious osascript paramaters within a a Python PIP execution. Python-pip is capabale of executing JavaScript code via osascript which can be abused by threat actors to backdoor Python packages.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS - Suspicious Python PIP Execution on {{device_hostname}} by {{user_username}}|
|Summary Expression|macOS - Suspicious Python PIP Execution on {{device_hostname}} by {{user_username}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.006|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


