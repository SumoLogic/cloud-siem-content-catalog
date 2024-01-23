# [Mappings](README.md): SentinelOne Logs - C2C activities

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|SentinelOne|
|Product|MGMT API|
|Log Format|JSON|
|Event ID Regex Pattern|`activities`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|SentinelOne|
|Product|SentinelOne|
|Record Type|Endpoint|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|accountId|accountId||
|description|primaryDescription||
|device_osName|osFamily||
|threat_identifier|threatId||
|user_username|data.username||

