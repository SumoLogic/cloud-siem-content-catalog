# [Mappings](README.md): Qualys Vulnerability Data

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Qualys|
|Product|VMScan|
|Log Format|JSON|
|Event ID Regex Pattern|`vulnerability_data`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Qualys|
|Product|VMScan|
|Record Type|NotificationVulnerability|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|device_hostname|Hostname||
|device_ip|IP||
|normalizedSeverity|None|The static text `0` is populated in this schema field.|
|severity|Detection.Severity||
|sourceUid|Id||
|threat_name|Detection.Results||
|threat_ruleType|None|The static text `direct` is populated in this schema field.|
|threat_signalName|Qualys Vulnerability Detected with Severity:%s||

