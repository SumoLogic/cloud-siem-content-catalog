# [Rules](README.md): AWS Bedrock - Knowledge Base Mass Deletion

## Description
Detection:
This rule triggers when a user deletes multiple AWS Bedrock Knowledge Bases within a short time period from the same source IP address. It monitors CloudTrail logs for successful DeleteKnowledgeBase API calls and excludes AWS service-linked roles,

Scenario:
An attacker who has gained access to an AWS account may attempt to disrupt AI/ML operations by mass-deleting Bedrock Knowledge Bases containing critical business data and embeddings. This destructive action causes immediate service disruption and potential data loss, requiring time-consuming restoration from backups or complete re-indexing of knowledge bases.

Recommended Actions:
Verify deletions were authorized by reviewing user_username and srcDevice_ip against known administrative activity, then check requestParameters.knowledgeBaseId to assess the scope. If unauthorized, contact the account owner to confirm and assess whether backups are needed for restoration.

Tuning Recommendations:
Create a match list named 'authorized_automation_accounts' for legitimate automation accounts performing bulk knowledge base management. Adjust the threshold from 3 to a higher value if your environment regularly performs legitimate bulk deletions during maintenance windows.

## Additional Details
|Detail|Value|
|----|----|
|Type|Threshold|
|Category|Impact|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|AWS Bedrock - Knowledge Base Mass Deletion|
|Summary Expression|User {{user_username}} from IP {{srcDevice_ip}} deleted multiple AWS Bedrock Knowledge Bases rapidly|
|Threshold Count|3|
|Threshold Window|T60M|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTechnique:T1485, _mitreAttackTactic:TA0040|
## Vendors and Products
- [Amazon AWS - CloudTrail](../products/033624b0-218e-4dcb-b93f-0f1fb1806c56.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|
|Normalized Schema|user_username_role|


