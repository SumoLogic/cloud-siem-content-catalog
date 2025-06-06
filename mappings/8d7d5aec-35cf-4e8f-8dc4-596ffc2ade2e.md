# [Mappings](README.md): Google G Suite - logout

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Google|
|Product|G Suite|
|Log Format|JSON|
|Event ID Regex Pattern|`login.logout\|login-login-logout`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Google|
|Product|G Suite|
|Record Type|Authentication|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|events.name||
|description|events.type||
|logonType|events.parameters.login_type||
|normalizedAction|None|The static text `logoff` is populated in this schema field.|
|srcDevice_ip|ipAddress||
|success|None|The static text `true` is populated in this schema field.|
|timestamp|id.time|We expect the orginal record value of `id.time` is in the format `yyyy-MM-dd'T'HH:mm:ss.SSSZ`|
|user_authDomain|ownerDomain||
|user_email|actor.email||
|user_userId|actor.profileId||
|user_username|actor.email|This is a split field. More info to come in the catalog later...|

