# [Rules](README.md): Autorun file created after USB disk mount on host

## Description
This signal looks for a USB drive being mounted on a Windows host followed by a file creation event with the file name of "autorun.inf" within a 5-minute time frame. This activity could be indicative of an attempt at lateral movement or initial access avenues through a USB device. Ensure that the machine in question is authorized to use USB devices and look for other file creation events from this host around the same time frame. This rule logic utilizes Sysmon file creation events, which need to be enabled and configured on relevant assets.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Lateral Movement|
|Apply Risk to Entities|device_hostname|
|Signal Name|Autorun file created after USB disk mount on host|
|Summary Expression|An autorun.inf was created on a USB device shortly after mounting the drive on  {{device_hostname}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0008, _mitreAttackTactic:TA0001, _mitreAttackTechnique:T1091|
## Vendors and Products
- [Microsoft - Windows](../products/1ff7546c-cb36-4a24-87f7-89d2cecc5761.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Direct from Record|fields["EventData.ClassName"]|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_vendor|


