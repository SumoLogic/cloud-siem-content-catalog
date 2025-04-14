# [Rules](README.md): GitHub - Audit Logging Modification

## Description
Detects modifications to the GitHub Enterprise Audit Log. Modifications and deletions have the potential to reduce visibility of malicious activity. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Defense Evasion|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GitHub - {{action}} performed by {{user_username}}|
|Summary Expression|{{user_username}} performed a {{normalizedAction}} activity on the {{fields['business']}} business audit log|
|Score/Severity|Dynamic: 0 or 3 or 5|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0005, _mitreAttackTechnique:T1562, _mitreAttackTechnique:T1562.008|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Dynamic Signal Score/Severity Translation

The default score of `0` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|audit_log_streaming.update|3|
|action|audit_log_streaming.destroy|5|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


