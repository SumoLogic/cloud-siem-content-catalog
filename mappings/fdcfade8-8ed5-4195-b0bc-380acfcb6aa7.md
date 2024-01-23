# [Mappings](README.md): Cisco Ironport WSA - Custom Parser

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|Cisco|
|Product|Ironport|
|Log Format|JSON|
|Event ID Regex Pattern|`TCP.*`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Cisco Systems|
|Product|Ironport|
|Record Type|NetworkProxy|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|action|transaction_result_code||
|device_ip|client_ip||
|http_category|url_category||
|http_method|connect_type||
|http_response_statusCode|http_response_code||
|http_url|dst_url||
|srcDevice_ip|client_ip||
|user_username|username||

