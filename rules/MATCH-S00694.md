# [Rules](README.md): Proofpoint POD Suspicious Email

## Description
Detects emails with a spam score greater than 50 using Proofpoint POD.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_hostname, srcDevice_ip, user_username, targetUser_username|
|Signal Name|Proofpoint POD Suspicious Email|
|Summary Expression|Email from {{email_sender}} to {{targetUser_email}} with subject {{email_subject}} has a spam score above 50.|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0009, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
## Vendors and Products
- [Proofpoint - Proofpoint on Demand](../products/332856e9-3111-446f-8df7-e64694e4b9a1.md)


## Fields Used

|Origin|Field|
|----|----|
|Direct from Record|fields['filter.modules.spam.scores.classifiers.impostor']|
|Direct from Record|fields['filter.modules.spam.scores.classifiers.malware']|
|Direct from Record|fields['filter.modules.spam.scores.classifiers.mlx']|
|Direct from Record|fields['filter.modules.spam.scores.classifiers.phish']|
|Direct from Record|fields['filter.modules.spam.scores.classifiers.spam']|
|Normalized Schema|metadata_product|
|Normalized Schema|metadata_vendor|
|Normalized Schema|srcDevice_hostname|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|targetUser_username|
|Normalized Schema|user_username|


