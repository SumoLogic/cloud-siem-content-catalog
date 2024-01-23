# [Rules](README.md): Zoom - Information Barrier Policy Changes

## Description
Monitors Zoom information barrier policy creations, deletions, and updates. nformation Barriers are designed to help customers control user communication policies and meet regulatory requirements at scale. They can be used to prevent certain groups of users with sensitive information from communicating with others who are not supposed to know of this information.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Exfiltration|
|Apply Risk to Entities|user_username|
|Signal Name|Zoom - Information Barrier Policy Changes - {{action}}|
|Summary Expression|User: {{user_username}} {{action}}|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0010|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_vendor|
|Normalized Schema|user_username|


