# [Rules](README.md): Chromium Browser History Access by Non-Browser Process

## Description
Chromium history files contain a wealth of information regarding browser usage patterns. Threat actors may enumerate Chromium history, bookmarks and cookies in order to extract sensitive information from systems.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname, user_username|
|Signal Name|Chromium Browser History Access by Non-Browser Process|
|Summary Expression|Non-browser process {{baseImage}} has accessed the Chromium history file {{file_path}} on {{device_hostname}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1555.003|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|baseImage|
|Normalized Schema|device_hostname|
|Normalized Schema|file_path|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


