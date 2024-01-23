# [Rules](README.md): Linux Host Entered Promiscuous Mode

## Description
Promiscuous mode causes a network interface to send all traffic frames it receives to the host's CPU rather than only the frames designated for the receiver. This is required for several packet sniffing tools, such as tcpdump or Wireshark, and should be scrutinized for legitimacy. Network administrators may need to be tuned out of this rule.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|device_hostname|
|Signal Name|Linux Host Entered Promiscuous Mode|
|Summary Expression|Host {{device_hostname}} entered promiscuous mode|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTactic:TA0007, _mitreAttackTechnique:T1040|
## Vendors and Products
- [Linux - Linux OS Syslog](../products/0e20c932-d992-4bd4-b276-c15119ca5c0b.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|device_hostname|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|


