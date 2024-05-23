# [Rules](README.md): First Seen USB device in use on Windows host

## Description
This signal looks for a new removable USB device name being used by a host not seen since the baseline period. This activity by itself is not necessarily malicious, but can be indicative of potential lateral movement or initial access tactics. If the device name is unexpected and not authorized to be used in the environment, investigate the alert further and look for file creation events to the drive in question. The fields["EventData.DeviceDescription"] field contains the device name.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname|
|Signal Name|First Seen USB device in use on Windows host: {{device_hostname}}|
|Summary Expression|A First Seen USB device found on {{device_hostname}}|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Baseline Type|PER_ENTITY|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1091|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Direct from Record|fields["EventData.ClassName"]|
|Direct from Record|fields["EventData.DeviceDescription"]|
|Normalized Schema|matches|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|


