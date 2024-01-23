# [Rules](README.md): macOS - Suspicious Osascript Execution and Network Activity

## Description
This rule utilizes Jamf telemetry and looks for osascript execution with a suspicious parent process indicating execution from a shell or terminal in addition to the osascript process making network connections to an external IP address.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Execution|
|Apply Risk to Entities|device_hostname|
|Signal Name|macOS - Suspicious Osascript Execution and Network Activity|
|Summary Expression|macOS - Suspicious Osascript Execution followed by osascript network connection to external IP on {{device_hostname}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1059.002|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|isNull|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|


