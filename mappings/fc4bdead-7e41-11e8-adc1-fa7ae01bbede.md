# [Mappings](README.md): Trend Micro LEEF logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Trend Micro|
|Product|Deep Security Agent|
|Log Format|LEEF|
|Event ID Regex Pattern|`_default_`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Trend Micro|
|Product|Deep Security|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|act||
|description|msg||
|device_ip|dvc||
|dstDevice_ip|dst||
|dstDevice_mac|dstMAC||
|dstPort|dstPort||
|file_basename|filePath||
|ipProtocol|proto||
|severity|sev||
|srcDevice_ip|src||
|srcDevice_mac|srcMAC||
|srcPort|srcPort||
|threat_name|cat||

