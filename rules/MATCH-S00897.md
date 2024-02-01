# [Rules](README.md): Chromium Extension Installed

## Description
Threat actors may install browser extensions as a form of persistence on victim systems. Look up the 32 character extension ID in order to ensure that the extension is valid and expected to be installed as part of normal business operations. This extension ID can be found in the following values: {{file_path}} and/or {{changeTarget}} depending on the source of the telemetry.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Persistence|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|A Chromium Extension was installed on {{device_hostname}} by {{user_username}}|
|Summary Expression|A Chromium Extension was installed on {{device_hostname}} by {{user_username}}  with the following path: {{file_path}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0003, _mitreAttackTechnique:T1176|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|changeTarget|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|user_username|


