# [Rules](README.md): GitHub - OAuth Application Activity

## Description
Detects OAuth application activities within GitHub. OAuth application management and access activity should be monitored for potential abuse by malicous actors, either by creating malicious access paths within GitHub, or destruction of GitHub infrastructure. This detection was developed utilizing GitHub Enterprise Audit logging. Refer to https://help.sumologic.com/docs/integrations/app-development/github/#collecting-logs-for-github for instructions on ingesting GitHub Enterprise Audit logs.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|user_username, srcDevice_ip|
|Signal Name|GitHub - {{user_username}}  Performed an {{action}} Operation|
|Summary Expression|OAuth operation: {{action}} performed by {{user_username}}within the {{fields['org']}} organization|
|Score/Severity|Dynamic: 1 or 2 or 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTactic:TA0003, _mitreAttackTactic:TA0006|
## Vendors and Products
- [Github - GitHub Enterprise Audit](../products/e3c8bd8b-6ed8-4332-944d-d0f5dfc462df.md)


## Dynamic Signal Score/Severity Translation

The default score of `1` is used as a catch all if none of the translations are met.

|Schema Field|Field Value|Score/Severity|
|------------|-----------|--------------|
|action|oauth_application.create|2|
|action|oauth_application.destroy|3|
|action|oauth_application.reset_secret|3|
|action|oauth_application.revoke_tokens|3|
|action|org.disable_oauth_app_restrictions|3|
|action|org.oauth_app_access_approved|2|
## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|action|
|Normalized Schema|metadata_product|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


