# [Rules](README.md): Zoom - Meeting Risk Alert

## Description
The At-Risk Meeting Notifier event is triggered every time someone posts a Zoom meeting link to a social media account, such as Reddit or Twitter.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Zoom - Meeting Risk Alert - {{action}}|
|Summary Expression|User: {{user_username}} {{action}}|
|Score/Severity|Static: 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010|
## Vendors and Products
- [Zoom - Zoom](../products/ad8d40a9-ee64-4615-bd92-aa964b4ae3b0.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


