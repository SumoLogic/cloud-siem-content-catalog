# [Rules](README.md): GCP IDS Detection Followed by API Call

## Description
Detects a GCP IDS hit followed by an API call, indicating the source IP was able to gain access to GCP.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|GCP IDS Detection Followed by API Call|
|Summary Expression|{{srcDevice_ip}} was seen using GCP API calls after IDS detection.|
|Score/Severity|Static: 6|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1212|
## Vendors and Products
- [Google - Google Cloud Platform](../products/dcc85cfc-a698-4d09-87de-f2c723f3ad07.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|metadata_deviceEventId|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


