# [Mappings](README.md): Alert Logic Catch All

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Alert Logic|
|Product|Alert Logic|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Alert Logic|
|Product|Alert Logic|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|account_id||
|action|Event Name||
|cloud_zone|Zone||
|description|summary||
|dstDevice_hostname|Target Hostname||
|dstPort|data.1.items.1.toPort||
|errorCode|error_message||
|ipProtocol|data.1.items.1.ipProtocol||
|normalizedAction|Event Name|This is a lookup field. More info to come in the catalog later...|
|normalizedResource|None|The static text `service` is populated in this schema field.|
|normalizedSeverity|threat_rating|This is a lookup field. More info to come in the catalog later...|
|resource|ARN||
|severity|threat_rating||
|srcDevice_hostname|attacker||
|srcPort|data.1.items.1.fromPort||
|success|Event Name|This is a lookup field. More info to come in the catalog later...|
|targetUser_username|victim||
|threat_identifier|long_incident_id||
|user_role|User Type||
|user_username|Username||

