# [Rules](README.md): Browser Exploitation Framework (BeEF) Hook

## Description
The Browser Exploitation Framework (BeEF) is a penetration-testing tool focusing on web browsers. This rule looks for HTTP communication that include the default BeEF cookie, which indicates a hooked browser.

## Additional Details
|Detail|Value|
|----|----|
|Type|Match|
|Category|Execution|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|Browser Exploitation Framework (BeEF) Hook|
|Summary Expression|BeEF hook detected from URL: {{http_url}} to destination host {{dstDevice_ip}}|
|Score/Severity|Static: 8|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0002, _mitreAttackTechnique:T1203|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|bro_http_request_headers['COOKIE']|
|Normalized Schema|bro_http_response_headers['SET-COOKIE']|
|Normalized Schema|srcDevice_ip|


