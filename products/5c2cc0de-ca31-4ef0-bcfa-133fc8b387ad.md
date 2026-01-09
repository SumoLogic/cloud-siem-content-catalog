# [Products](README.md): Jamf - Jamf

## Rules

|Rule ID|Rule Name|
|----|----|
|MATCH-S00686|[Base64 Decode in Command Line](../rules/MATCH-S00686.md)|
|MATCH-S00269|[Clipboard Copied](../rules/MATCH-S00269.md)|
|MATCH-S00348|[Curl Start Combination](../rules/MATCH-S00348.md)|
|FIRST-S00028|[First Seen Common Windows Recon Commands From User](../rules/FIRST-S00028.md)|
|FIRST-S00042|[First Seen Ioreg Usage from User](../rules/FIRST-S00042.md)|
|FIRST-S00032|[First Seen Kubectl Command From User](../rules/FIRST-S00032.md)|
|FIRST-S00030|[First Seen Outbound Connection to External IP Address on Port 445 from IP Address](../rules/FIRST-S00030.md)|
|FIRST-S00038|[First Seen Wget Usage from User](../rules/FIRST-S00038.md)|
|FIRST-S00040|[First Seen cURL execution from User](../rules/FIRST-S00040.md)|
|FIRST-S00039|[First Seen mdfind Usage from User](../rules/FIRST-S00039.md)|
|FIRST-S00041|[First Seen networksetup Usage from User](../rules/FIRST-S00041.md)|
|FIRST-S00043|[First Seen pbpaste Usage from User](../rules/FIRST-S00043.md)|
|MATCH-S00702|[Keychain Credential Dumping](../rules/MATCH-S00702.md)|
|MATCH-S00648|[Kubernetes ListSecrets](../rules/MATCH-S00648.md)|
|MATCH-S00647|[Kubernetes Pod Deletion](../rules/MATCH-S00647.md)|
|MATCH-S00837|[Kubernetes Secrets Enumeration via Kubectl](../rules/MATCH-S00837.md)|
|MATCH-S00687|[Linux Security Tool Usage](../rules/MATCH-S00687.md)|
|MATCH-S00534|[MacOS - Re-Opened Applications](../rules/MATCH-S00534.md)|
|MATCH-S00729|[MacOS Gatekeeper Bypass](../rules/MATCH-S00729.md)|
|MATCH-S00402|[Normalized Security Signal](../rules/MATCH-S00402.md)|
|MATCH-S00554|[Outbound IRC Traffic](../rules/MATCH-S00554.md)|
|MATCH-S00683|[Overly Permissive Chmod Command](../rules/MATCH-S00683.md)|
|MATCH-S00698|[PATH Set to Current Directory](../rules/MATCH-S00698.md)|
|AGGREGATION-S00004|[Suspicious K8s Enumeration](../rules/AGGREGATION-S00004.md)|
|AGGREGATION-S00005|[Suspicious System Enumeration Occurring in Quick Succession](../rules/AGGREGATION-S00005.md)|
|MATCH-S00886|[Suspicious chmod Execution](../rules/MATCH-S00886.md)|
|MATCH-S01007|[Threat Intel - Destination Device Hostname](../rules/MATCH-S01007.md)|
|MATCH-S01024|[Threat Intel - Destination IP Address (High Confidence)](../rules/MATCH-S01024.md)|
|MATCH-S01006|[Threat Intel - Device Hostname](../rules/MATCH-S01006.md)|
|MATCH-S00555|[Threat Intel - Inbound Traffic Context](../rules/MATCH-S00555.md)|
|LEGACY-S00107|[Threat Intel Match - IP Address](../rules/LEGACY-S00107.md)|
|MATCH-S00880|[macOS - Entitlement Enumeration via Xattr](../rules/MATCH-S00880.md)|
|MATCH-S00883|[macOS - Keychain Enumeration](../rules/MATCH-S00883.md)|
|MATCH-S00885|[macOS - Screen Sharing Session Established](../rules/MATCH-S00885.md)|
|MATCH-S00879|[macOS - Suspicious Osascript Execution](../rules/MATCH-S00879.md)|
|CHAIN-S00016|[macOS - Suspicious Osascript Execution and Network Activity](../rules/CHAIN-S00016.md)|
|MATCH-S00878|[macOS - Suspicious Osascript Parent Execution](../rules/MATCH-S00878.md)|
|MATCH-S00884|[macOS - Suspicious Python PIP Execution](../rules/MATCH-S00884.md)|
|MATCH-S00882|[macOS - System Preference Enumeration via Security Binary](../rules/MATCH-S00882.md)|
|MATCH-S00881|[macOS - csrutil status Usage Detected](../rules/MATCH-S00881.md)|
|MATCH-S00726|[macOS Kernel Extension Load](../rules/MATCH-S00726.md)|


## Log Mappers

|Log Mapper ID|Log Mapper Name|
|----|----|
|833d135d-6811-4bf8-a73e-633aaba65cbf|[Jamf Audit User - Audit](../mappings/833d135d-6811-4bf8-a73e-633aaba65cbf.md)|
|7c8b105b-0a52-4f24-9c8e-4031c5389f72|[Jamf Audit User - Authentication](../mappings/7c8b105b-0a52-4f24-9c8e-4031c5389f72.md)|
|818d5001-4366-4c38-99b8-699b1ee5faab|[Jamf Audit User - Endpoint](../mappings/818d5001-4366-4c38-99b8-699b1ee5faab.md)|
|b7666280-63a6-414f-bf31-e274f766b9fd|[Jamf Audit User - Network](../mappings/b7666280-63a6-414f-bf31-e274f766b9fd.md)|
|0a0f1a7e-1019-4862-8bb4-6df7ff99f3d3|[Jamf Parser - Alert](../mappings/0a0f1a7e-1019-4862-8bb4-6df7ff99f3d3.md)|
|671b5df7-c62b-4c38-b12b-ace97c48f035|[Jamf Parser - Catch All](../mappings/671b5df7-c62b-4c38-b12b-ace97c48f035.md)|
|c389482c-8691-4320-bc52-d0110d759502|[Jamf Parser - Network](../mappings/c389482c-8691-4320-bc52-d0110d759502.md)|
|220de41a-b2a3-4ec6-ace6-ae26a9b4f04f|[Jamf Protect Analytics - Events](../mappings/220de41a-b2a3-4ec6-ace6-ae26a9b4f04f.md)|


