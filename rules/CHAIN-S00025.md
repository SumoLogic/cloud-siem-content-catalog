# [Rules](README.md): OpenClaw - Installation Detected via DNS

## Description
Detection:
This chain rule triggers when a device makes a high number of DNS queries for messaging platform domains (Telegram, Discord, Slack, Teams, etc.) and AI service domains (OpenAI, Anthropic, HuggingFace, etc.) within 24 hours. 

Scenario:
OpenClaw is an agentic AI framework which may either be unsanctioned or tightly controlled in your environment, and a user has installed OpenClaw without approval. The host on which OpenClaw is installed may not be under IT control. 

Recommended Actions:
Investigate srcDevice_ip to identify the user, then review endpoint logs for OpenClaw artifacts (file writes, port 18789 websockets, node shell processes). If unauthorized, remove the installation.

Tuning Recommendations:
Create match list 'authorized_openclaw_devices' for permitted systems, and adjust thresholds upward if legitimate Slack/Teams integrations generate false positives. Combine with other OpenClaw detections for comprehensive coverage.

## Additional Details
|Detail|Value|
|----|----|
|Type|Chain|
|Category|Unknown/Other|
|Apply Risk to Entities|srcDevice_ip|
|Signal Name|OpenClaw - Installation Detected via DNS|
|Summary Expression|Possible OpenClaw installation detected on host {{srcDevice_ip}}|
|Score/Severity|Static: 1|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAtlasTechnique:AML.T0103, _mitreAtlasTactic:AML.TA0005|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dns_query|
|Normalized Schema|srcDevice_ip|


