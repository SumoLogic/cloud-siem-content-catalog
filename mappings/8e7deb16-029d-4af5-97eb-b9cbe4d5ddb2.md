# [Mappings](README.md): Proofpoint TRAP Default Mapping

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Proofpoint|
|Product|TRAP|
|Log Format|JSON|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Proofpoint|
|Product|TRAP|
|Record Type|Email|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|----------------|-------------------|-----|
|accountId|tenant_id||
|description|incidents.1.title||
|email_messageId|message_id||
|email_sender|sender_address||
|email_subject|email_subject||
|flowState|remediation_status||
|normalizedSeverity|clear_confidence|This is a lookup field. More info to come in the catalog later...|
|severity|clear_confidence||
|success|message_status.message_delivered||
|targetUser_email|recipient_address||
|targetUser_username|recipient_address|This is a split field. More info to come in the catalog later...|
|threat_category|tap_threat_types.1||
|threat_identifier|incidents.1.id||
|threat_name|incidents.1.title||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|incidents.1.title||
|user_email|sender_address||
|user_username|sender_address|This is a split field. More info to come in the catalog later...|

