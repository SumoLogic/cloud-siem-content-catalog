# [Mappings](README.md): DataBricks Audit Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Databricks|
|Product|Databricks Audit|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Databricks|
|Product|Databricks Audit|
|Record Type|AuditChange|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|account_id||
|action|action_name||
|email_subject|subject_name||
|errorText|error_message||
|http_response_statusCode|status_code||
|http_userAgent|user_agent||
|normalizedAction|action_name|This is a lookup field. More info to come in the catalog later...|
|sessionId|session_id||
|srcDevice_ip|source_ip_address||
|user_email|user_email||
|user_userId|user_id||
|user_username|user_email|This is a split field. More info to come in the catalog later...|

