# [Rules](README.md): AWS EKS Failed Curl Authentication Attempt

## Description
Failed instances of curl usage within a containerized environment should occur rarely, investigate the source IP address used to ensure that it is legitimate.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|AWS EKS Failed Curl Authentication Attempt|
|Summary Expression|A failed authentication attempt to an AWS EKS cluster using the curl utility has been in association with the following IP: {{srcDevice_ip}}|
|Score/Severity|Static: 0|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1609, _mitreAttackTactic:TA0002|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.responseStatus.status"]|
|Direct from Record|fields["message.user.groups.1"]|
|Normalized Schema|srcDevice_ip|


