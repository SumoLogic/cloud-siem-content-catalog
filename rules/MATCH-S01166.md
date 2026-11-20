# [Rules](README.md): AI Model Downloaded from Public Repository

## Description
Detection: This rule triggers when a network request names an AI model file extension (.pkl, .pt, .pth, .bin, .gguf, .safetensors, .ckpt, .joblib, .onnx, .h5) on a known model repository host, fetches a content-addressed object from a model repository content delivery network, or pulls from a model registry or download endpoint.

Scenario: Models pulled from public repositories can carry executable payloads, and attackers have published weaponized models and typosquatted names to reach organizations that adopt them. This rule shows which endpoints are pulling models from public sources.

Recommended Actions: Identify the user and host that fetched the object and whether it was part of an approved workflow. Check the repository and file name where the path names one.

Tuning Recommendations: To exclude approved model sources, create a match list named allowed_ai_domains under Cloud SIEM > Match Lists, set its target column to Domain, and add the approved domains; this rule already excludes records that match it.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Initial Access|
|Apply Risk to Entities|srcDevice_ip, user_username, device_hostname|
|Signal Name|AI Model Downloaded from {{http_url_fqdn}}|
|Summary Expression|AI model downloaded from {{http_url_fqdn}} by {{user_username}} from {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0001, _mitreAttackTechnique:T1195, _mitreAtlasTactic:AML.TA0004, _mitreAtlasTechnique:AML.T0010.003|
## Vendors and Products
- [Squid - Squid Proxy](../products/af61d8a8-3eba-42fb-9f17-87443924f3f4.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|device_hostname|
|Normalized Schema|http_url_fqdn|
|Normalized Schema|http_url_path|
|Normalized Schema|http_url_rootDomain|
|Normalized Schema|srcDevice_ip|
|Normalized Schema|user_username|


