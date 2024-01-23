# [Mappings](README.md): Salesforce Normalized Security Signal Passthrough

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Salesforce|
|Product|Salesforce|
|Log Format|JSON|
|Event ID Regex Pattern|`ApiAnomalyEvent.*\|ReportAnomalyEvent.*\|CredentialStuffingEvent.*\|SessionHijackingEvent.*`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Salesforce|
|Product|Salesforce|
|Record Type|Audit|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|api_type||
|application|Section||
|description|Display||
|http_method|METHOD||
|http_response_contentType|MEDIA_TYPE||
|http_response_statusCode|STATUS_CODE||
|http_userAgent|USER_AGENT||
|normalizedSeverity|None|The static text `3` is populated in this schema field.|
|srcDevice_ip|source_ip||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|Action||
|user_userId|user_id||
|user_username|username||

