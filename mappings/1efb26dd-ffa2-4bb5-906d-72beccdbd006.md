# [Mappings](README.md): AWS - Application Load Balancer - Connection

## Input Requirements

|Input|Value|
|-----|-----|
|Vendor|AWS|
|Product|Application Load Balancer|
|Log Format|JSON|
|Event ID Regex Pattern|`AWS_ALB_CONN`|

## Record Output

|Output|Value|
|------|-----|
|Vendor|Amazon AWS|
|Product|Application Load Balancer|
|Record Type|Network|

## Fields Mapped

|Cloud SIEM Schema Field|Original Record Key|Notes|
|-----------------------|-------------------|-----|
|cloud_provider|None|The static text `AWS` is populated in this schema field.|
|cloud_service|None|The static text `Application Insights` is populated in this schema field.|
|dstPort|listener_port||
|srcDevice_ip|client_ip||
|srcPort|client_port||
|success|tls_verify_status|This is a lookup field. More info to come in the catalog later...|

