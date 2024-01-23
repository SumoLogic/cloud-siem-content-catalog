# [Rules](README.md): macOS - Screen Sharing Session Established

## Description
This rule utilizes Jamf telemetry and looks for a successful screen sharing connection to a macOS host. The username that performed the connection is located within the "texts.1" field - ensure that this remote connection activity is authorized.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS - Screen Sharing Session Established on {{device_hostname}}|
|Summary Expression|macOS - Screen Sharing Session Established on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTechnique:T1021.005|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|errorCode|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|parentBaseImage|


