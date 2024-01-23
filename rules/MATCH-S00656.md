# [Rules](README.md): Unrecognized Container Image

## Description
Monitors for unrecognized container images that may indicate an attempt to bypass security controls on existing images or escalate privileges. This rule is disabled by default to allow for proper configuration of the match lists used to determine recognized images.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username|
|Signal Name|Unrecognized Container Image|
|Summary Expression|Unrecognized container image: {{resource}}|
|Score/Severity|Static: 1|
|Enabled by Default|False|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1525|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|listMatches|
|Normalized Schema|metadata_product|
|Normalized Schema|resource|
|Normalized Schema|user_username|


