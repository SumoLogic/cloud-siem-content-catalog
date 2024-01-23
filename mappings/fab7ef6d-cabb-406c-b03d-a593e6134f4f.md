# [Mappings](README.md): CrowdStrike FDR - ProcessRollup2

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|CrowdStrike|
|Product|FDR|
|Log Format|JSON|
|Event ID Regex Pattern|`ProcessRollup2`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|CrowdStrike|
|Product|FDR|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|UserSid||
|baseImage|ImageFileName||
|commandLine|CommandLine||
|device_hostname|ComputerName||
|device_ip|aip||
|device_uniqueId|aid||
|file_hash_md5|MD5HashData||
|file_hash_sha256|SHA256HashData||
|file_path|ImageFileName||
|parentBaseImage|ParentBaseFileName||
|user_username|UserSid||

