# [Rules](README.md): Suspicious Email Attachment Extension

## Description
Observes for e-mail attachments with file extensions commonly used by attackers or associated with malware.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username|
|Signal Name|Suspicious Email Attachment Extension|
|Summary Expression|Suspicious email attachment from: {{email_sender}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0009, _mitreAttackTactic:TA0043, _mitreAttackTechnique:T1566, _mitreAttackTechnique:T1566.001, _mitreAttackTechnique:T1566.002, _mitreAttackTechnique:T1598, _mitreAttackTechnique:T1598.002, _mitreAttackTechnique:T1598.003|
## Vendors and Products
- [Microsoft - Azure](../products/a1225af5-e778-4068-a9a2-47da93d1ff24.md)
- [Microsoft - Defender Advanced Hunting](../products/3382523e-2072-41bd-b50b-6b148957d0b0.md)
- [Microsoft - Office 365](../products/d3ed003d-5ddd-4c7a-bea5-63eae6311833.md)
- [Proofpoint - Proofpoint on Demand](../products/332856e9-3111-446f-8df7-e64694e4b9a1.md)
- [Proofpoint - Targeted Attack Protection](../products/de3d4b6b-36a3-4436-8bfc-0561ac95037e.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|file_basename|
|Normalized Schema|file_path|
|Normalized Schema|objectType|
|Normalized Schema|user_username|


