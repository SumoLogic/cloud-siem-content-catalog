# [Rules](README.md): AWS CloudTrail - Public S3 Bucket Exposed

## Description
An AWS request occurred to either create a new public bucket or to add a bucket access control list (ACL) to an existing bucket to make it public. While there are some use cases for AWS S3 public buckets, most are generally private. The security operations center should have a strong understanding of which buckets are allowed to be public.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|device_hostname, device_ip, user_username, srcDevice_ip|
|Signal Name|AWS CloudTrail - Public S3 Bucket Exposed|
|Summary Expression|S3 Bucket {{changeTarget}} has been placed in an ACL allowing it to be publicly exposed|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0009, _mitreAttackTechnique:T1530|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|application|
|Normalized Schema|device_hostname|
|Normalized Schema|device_ip|
|Direct from Record|fields['requestParameters.AccessControlPolicy.AccessControlList.Grant.1.Grantee.URI']|
|Direct from Record|fields['requestParameters.AccessControlPolicy.AccessControlList.Grant.2.Grantee.URI']|
|Direct from Record|fields['requestParameters.AccessControlPolicy.AccessControlList.Grant.3.Grantee.URI']|
|Direct from Record|fields['requestParameters.AccessControlPolicy.AccessControlList.Grant.4.Grantee.URI']|
|Direct from Record|fields['requestParameters.AccessControlPolicy.AccessControlList.Grant.5.Grantee.URI']|
|Direct from Record|fields['requestParameters.x-amz-acl']|
|Direct from Record|fields['requestParameters.x-amz-grant-read']|
|Direct from Record|fields['requestParameters.x-amz-grant-read-acp']|
|Direct from Record|fields['requestParameters.x-amz-grant-write']|
|Direct from Record|fields['requestParameters.x-amz-grant-write-acp']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


