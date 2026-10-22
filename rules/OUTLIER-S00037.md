# [Rules](README.md): Spike in HTTP Server Errors to Destination IP

## Description
Detection: This rule detects a statistically significant spike in HTTP 5xx server error responses returned by a known web server, relative to that server's own 30-day historical baseline.

Scenario: A sudden spike in server errors can indicate an exploitation attempt causing application failures, a misconfiguration or deployment regression, or a denial-of-service condition degrading availability.

Requirements: The web_servers and/or http_servers match lists must be populated with the IP addresses of the web servers to monitor, and HTTP logs from those servers (for example Zeek HTTP, or web server access logs) must be ingested with the HTTP response status code and destination IP normalized. If both lists are empty, this rule will not fire.

Recommended Actions: Review recent changes or deployments to the destination host, correlate with source IPs generating the errors, and check whether a narrow set of URLs/paths is driving the spike versus broad failure across the service.

Tuning Recommendations: Scoped to the web_servers and http_servers match lists so only known web server destinations are evaluated.

## Additional Details
|Detail|Value|
|----|----|
|Type|Outlier|
|Category|Impact|
|Apply Risk to Entities|dstDevice_ip|
|Signal Name|Spike in HTTP Server Errors to Destination IP: {{dstDevice_ip}}|
|Summary Expression|An outlier in HTTP server error responses to destination IP: {{dstDevice_ip}} has been detected|
|Retention Window|7776000000|
|Baseline Window|2592000000|
|Standard Deviation Threshold|2|
|Floor Value|5|
|Score/Severity|Static: 3|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAttackTactic:TA0040, _mitreAttackTechnique:T1499|
## Vendors and Products


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|http_response_statusCode|


