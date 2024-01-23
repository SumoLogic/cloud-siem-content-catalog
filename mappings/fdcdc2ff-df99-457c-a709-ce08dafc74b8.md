# [Mappings](README.md): Bitdefender - new-incident

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Bitdefender|
|Product|GravityZone|
|Log Format|JSON|
|Event ID Regex Pattern|`new-incident`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Bitdefender|
|Product|GravityZone|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|params.events.main_action||
|baseImage|params.events.file_path||
|commandLine|params.events.process_command_line||
|device_hostname|params.events.computer_name||
|device_ip|params.events.computer_ip||
|file_hash_md5|params.events.file_hash_md5||
|file_hash_sha256|params.events.file_hash_sha256||
|normalizedSeverity|params.events.severity|This is a lookup field. More info to come in the catalog later...|
|parentBaseImage|params.events.parent_process_path||
|pid|params.events.process_pid||
|severity|params.events.severity||
|srcDevice_ip|params.events.source_ip||
|threat_name|params.events.detection_name||
|threat_ruleType|params.events.severity||
|threat_signalName|params.events.detection_name||
|user_userId|params.events.user_sid||
|user_username|params.events.username||

