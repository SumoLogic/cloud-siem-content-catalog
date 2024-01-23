# [Mappings](README.md): SentinelOne Logs - C2C alerts

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|SentinelOne|
|Product|MGMT API|
|Log Format|JSON|
|Event ID Regex Pattern|`alerts`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|SentinelOne|
|Product|SentinelOne|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|baseImage|sourceProcessInfo.name||
|commandLine|sourceProcessInfo.commandline||
|description|ruleInfo.description||
|device_hostname|agentDetectionInfo.name||
|device_osName|agentDetectionInfo.osFamily||
|file_hash_md5|sourceProcessInfo.fileHashMd5||
|file_hash_sha1|sourceProcessInfo.fileHashSha1||
|file_hash_sha256|sourceProcessInfo.fileHashSha256||
|file_path|sourceProcessInfo.filePath||
|normalizedSeverity|ruleInfo.severity|This is a lookup field. More info to come in the catalog later...|
|parentCommandLine|sourceParentProcessInfo.commandline||
|severity|ruleInfo.severity|This is a lookup field. More info to come in the catalog later...|
|threat_identifier|ruleInfo.id||
|threat_name|ruleInfo.name||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|ruleInfo.name||
|user_username|sourceProcessInfo.user||

