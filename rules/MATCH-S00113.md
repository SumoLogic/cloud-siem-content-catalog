# [Rules](README.md): AWS CloudTrail - Logging Configuration Change Observed

## Description
Changing the configuration of logging to any mission-critical service or platform should be closely monitored.  This signal identifies when AWS logging configurations have been changed.  The severity of signals increases depending on the type of action observed.  For instance disabling/deleting logs is a higher severity than enabling logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Logging Configuration Change Observed|
|Summary Expression|{{action}} performed by user: {{user_username}}|
|Score/Severity|Dynamic: 1 or 2 or 4|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTactic:TA0005, _mitreAttackTechnique:T1489, _mitreAttackTechnique:T1578, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1578.004, _mitreAttackTechnique:T1562.008|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|metadata_deviceEventId|AwsApiCall-CreateTrail|1|
|metadata_deviceEventId|AwsApiCall-UpdateTrail|2|
|metadata_deviceEventId|AwsApiCall-DeleteTrail|4|
|metadata_deviceEventId|AwsApiCall-StartLogging|1|
|metadata_deviceEventId|AwsApiCall-StopLogging|4|
|metadata_deviceEventId|AwsApiCall-DeleteLogGroup|4|
|metadata_deviceEventId|AwsApiCall-DeleteLogStream|4|
|metadata_deviceEventId|AwsApiCall-DeleteDestination|4|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


