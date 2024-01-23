# [Mappings](README.md): Cisco Meraki IDS - Custom Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|Meraki|
|Log Format|JSON|
|Event ID Regex Pattern|`ids-alerts\|ids_alerted`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Meraki|
|Record Type|NetworkHTTP|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|description|message||
|dstDevice_hostname|dhost||
|dstDevice_ip|dst||
|dstPort|dport||
|ipProtocol|protocol||
|normalizedSeverity|priority|This is a lookup field. More info to come in the catalog later...|
|severity|priority||
|srcDevice_hostname|shost||
|srcDevice_ip|src||
|srcPort|sport||
|threat_name|message||
|threat_ruleType|None|The static text `intrusion` is populated in this schema field.|
|timestamp|syslog_timestamp|We expect the orginal record value of `syslog_timestamp` is in the format `epoch_float`|

