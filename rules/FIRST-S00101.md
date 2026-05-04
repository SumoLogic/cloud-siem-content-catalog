# [Rules](README.md): AWS Bedrock - KB Data Source from External S3 Bucket

## Description
Detection:
This rule triggers when an S3 bucket from an external AWS account is added to a Bedrock Knowledge Base via UpdateDataSource or CreateDataSource API calls in which the external AWS account hasn't been observed in the last 90 days.

Scenario:
An attacker with Bedrock permissions may poison a RAG system by adding data sources from an external AWS account they control, injecting malicious content into the knowledge base without compromising the organization's S3 buckets. This RAG poisoning technique enables data manipulation, misinformation injection, or credential harvesting through malicious AI responses.

Recommended Actions:
Verify the cross-account bucket addition is authorized by reviewing user_username and checking if bucketOwnerAccountId belongs to your organization or a trusted partner. If unauthorized, remove the external data source immediately, revoke IAM permissions, and audit all Knowledge Base configurations for additional modifications.

Tuning Recommendations:
Create a match list named 'authorized_bedrock_external_accounts' containing trusted AWS account IDs for cross-account data sharing. For organizations that never use cross-account S3 buckets with Bedrock, this rule can run without exclusions.

## Additional Details
|Detail|Value|
|----|----|
|Type|First Seen|
|Category|Unknown/Other|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|AWS Bedrock Knowledge Base external data source added by {{user_username}}|
|Summary Expression|{{user_username}} added external data source from account {{fields['responseElements.dataSource.dataSourceConfiguration.s3Configuration.bucketOwnerAccountId']}} to Bedrock Knowledge Base from IP {{srcDevice_ip}}|
|Retention Window|7776000000|
|Baseline Window|0|
|Baseline Type|GLOBAL|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAtlasTechnique:AML.T0070, _mitreAtlasTactic:AML.TA0006|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Direct from Record|fields['responseElements.dataSource.dataSourceConfiguration.s3Configuration.bucketOwnerAccountId']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


