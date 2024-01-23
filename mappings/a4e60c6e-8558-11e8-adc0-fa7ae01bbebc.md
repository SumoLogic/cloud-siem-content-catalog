# [Mappings](README.md): Endgame CEF mapping

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Endgame|
|Product|Endgame|
|Log Format|CEF|
|Event ID Regex Pattern|`kernelShellcodeEventResponse\|fileClassificationEventResponse\|rulesEngineEventResponse\|Test alert`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Endgame|
|Product|Detection|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|cat||
|description|msg||
|device_hostname|dvchost||
|device_ip|dvc||
|file_basename|fname||
|file_path|filePath||
|severity|cfp1||
|threat_name|cat||
|timestamp|rt|We expect the orginal record value of `rt` is in the format `epoch_ms`|

