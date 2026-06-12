# [Rules](README.md): Openclaw - Activity on Default Port

## Description
Detection:
This rule triggers when a websocket connection to TCP port 18789 returns HTTP status 'Switching Protocols', indicating websocket handshake. Port 18789 is OpenClaw's default local server port, providing detection of active OpenClaw usage.

Scenario:
OpenClaw may be disallowed or tightly controlled in the organization. If a user installs OpenClaw on a device outside of IT control there may not be any telemetry on the device and network telemetry will be needed to detect unsanctioned installations. 

Recommended Actions:
Confirm OpenClaw is running on dstDevice_ip by checking for node processes on port 18789, then review network logs for external service communications (OpenAI, Anthropic). If unauthorized, terminate the process, remove the installation, block port 18789 at the firewall, and assess what code was processed.

Tuning Recommendations:
Create match list 'authorized_openclaw_devices' for permitted systems or other known services using port 18789.

## Additional Details
|Detail|Value|
|----|----|
|Type|Templated Match|
|Category|Unknown/Other|
|Apply Risk to Entities|dstDevice_ip|
|Signal Name|OpenClaw websocket detected on {{dstDevice_ip}}|
|Summary Expression|OpenClaw websocket connection detected on port 18789 to {{dstDevice_ip}}|
|Score/Severity|Static: 2|
|Enabled by Default|True|
|Prototype|False|
|Tags|_mitreAtlasTechnique:AML.T0103, _mitreAtlasTactic:AML.TA0005|
## Vendors and Products
- [Bro - Bro](../products/37C866BF-72E1-470A-9072-EDB908F56951.md)


## Fields Used

|Origin|Field|
|----|----|
|Normalized Schema|dstDevice_ip|
|Normalized Schema|dstPort|
|Normalized Schema|http_response_statusText|


