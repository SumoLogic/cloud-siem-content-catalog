# [Mappings](README.md): JFrog Artifactory - Login Access logs

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|JFrog|
|Product|Artifactory|
|Log Format|JSON|
|Event ID Regex Pattern|`access_logs-ACCEPTED_LOGIN\|access_logs-DENIED_LOGIN`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|JFrog|
|Product|Artifactory|
|Record Type|Authentication|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|event||
|file_path|repo_path||
|normalizedAction|logon||
|resource|repo_path||
|srcDevice_ip|ip||
|success|action|This is a lookup field. More info to come in the catalog later...|
|user_username|user||

