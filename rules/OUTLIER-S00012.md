# [Rules](README.md): Outlier in Data Inbound per Hour

## Description
A larger than typical amount of data inbound (bytesIn) has been observed exchanged with this source IP address. It is recommended to investigate the device associated with this IP, the Internet destinations and traffic associated with this anomalous behavior. A normalized record search for the source IP and external network traffic, within the period of time of the detection will help identify suspicious activity and Internet destinations.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Exfiltration|
|Apply Risk to Entities|srcDevice_ip, user_username|
|Signal Name|Outlier in Data Inbound per Hour - {{srcDevice_ip}}|
|Summary Expression|A larger than typical amount of data was observed inbound (bytesIn) to {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|1209600000|
|Standard Deviation Threshold|3|
|Floor Value|1000000000|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010, _mitreAttackTechnique:T1030|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bytesIn|
|Normalized Schema|dstDevice_ip_isInternal|
|Normalized Schema|objectClassification|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|srcDevice_ip_isInternal|
|Normalized Schema|user_username|


