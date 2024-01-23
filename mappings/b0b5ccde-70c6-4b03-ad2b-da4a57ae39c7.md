# [Mappings](README.md): BigQuery Gmail C2C - Error in Delivery

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Google|
|Product|Google Cloud Platform|
|Log Format|JSON|
|Event ID Regex Pattern|`14`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Google|
|Product|Google Cloud Platform|
|Record Type|Email|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|None|The static text `Error in Delivery` is populated in this schema field.|
|description|None|The static text `A temporary error occurred when Gmail tried to deliver the message, and the message has been scheduled for retry. This is usually caused by external or internal servers that are temporarily unavailable.` is populated in this schema field.|
|email_messageId|message_info.rfc2822_message_id||
|email_sender|message_info.source.address||
|email_subject|message_info.subject||
|file_basename|message_info.attachment||
|file_hash_sha256|message_info.attachment.sha256||
|file_mimeType|message_info.structured_policy_log_info.detected_file_types.mime_type||
|srcDevice_ip|message_info.connection_info.client_ip||
|success|None|The static text `false` is populated in this schema field.|
|threat_identifier|message_info.spam_info.disposition|This is a lookup field. More info to come in the catalog later...|
|threat_name|message_info.spam_info.classification_reason|This is a lookup field. More info to come in the catalog later...|
|threat_referenceUrl|message_info.link_domain||
|timestamp|event_info.timestamp_usec|We expect the orginal record value of `event_info.timestamp_usec` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSZ`|
|user_email|message_info.destination.address||
|user_username|message_info.destination.address||

