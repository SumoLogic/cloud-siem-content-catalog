# [Rules](README.md): Trufflehog AWS Credential Verification Detected

## Description
Trufflehog is a tool that can be utilized to find and verify secrets. When Trufflehog locates AWS credentials, it attempts to validate them using the GetCallerIdentity API call. This signal looks for the default Trufflehog User Agent within CloudTrail telemetry, combined with the GetCallerIdentity API call. Within this telemetry, the user_username field will contain the value of the username associated with the secret or credential that Trufflehog is attempting to verify. Look at the events surrounding the source IP address of this event. Look for any potential areas that may have contained keys or secrets for the user_username value.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Credential Access|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Trufflehog AWS Credential Verification Detected|
|Summary Expression|Trufflehog AWS Credential Verification Detected for {{user_username}}  from IP: {{srcDevice_ip}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0006, _mitreAttackTechnique:T1552|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|http_userAgent|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|


