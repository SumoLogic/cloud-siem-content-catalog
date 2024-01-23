# [Rules](README.md): Privileged Pod Created on AWS EKS

## Description
Privileged containers have all capabilities of the host machine. These privileged containers may perform actions directly on the host that they are running on. Ensure that this event is expected and occurs from a user account or IP address that normally works with privileged containers within the cluster. Customers are encouraged to set up an exclusion list for spec.securitycontext.capabilities for pods that are frequently going to be managed with privileged escalation.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Privilege Escalation|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Privileged Pod Created on AWS EKS by {{srcDevice_ip}}|
|Summary Expression|Privileged Pod Created on AWS EKS by {{srcDevice_ip}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0004, _mitreAttackTechnique:T1611|
## Vendors and Products
- [Amazon AWS - EKS](../products/234ec2b5-4142-4837-bc78-95da8a2db81a.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|admit-policy"]|
|Normalized Schema|cloud_provider|
|Normalized Schema|cloud_service|
|Direct from Record|fields["message.requestObject.spec.containers.1.securityContext.privileged"]|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|validate-policy"]|


