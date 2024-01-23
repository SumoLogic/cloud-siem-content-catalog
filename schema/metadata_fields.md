# [Schema](README.md): Metadata Fields

This lists all of the schema metadata fields automatically populated by Cloud SIEM.

|Field|Type|Description|
|-----|----|-----------|
|day|int|Day pulled from the timestamp.|
|hour|int|Hour pulled from the timestamp.|
|metadata_defaultTz|int|Default timezone for timestamp parsing|
|metadata_deviceEventId|string|Vendor specific event identifier. Is provided in the parser output and determines which mapping will be used.|
|metadata_mapperName|string|CSE mapper name which normalizes the record.|
|metadata_mapperUid|string|Universally unique identifier for CSE normalization mappers.|
|metadata_orgId|string|The Sumo Customer Org ID that originated the raw log message.|
|metadata_parseTime|long|The time at which the log line was parsed into a record by the parser and mapper service in milliseconds since epoch|
|metadata_parser|string|Name of the parser which extracted fields from the original log message.|
|metadata_product|string|The specific product name of the data source.|
|metadata_productGuid|string|Globally unique identifier for the combined vendor and product.|
|metadata_receiptTime|long|The time at which the log line was received by the collector in milliseconds since epoch|
|metadata_relayHostname|string|(Deprecated) Hostname of the syslog server that forwarded the log to the Sumo Logic sensor.|
|metadata_relayIp|string|(Deprecated) IP address of the syslog server that forwarded the log to the Sumo Logic sensor.|
|metadata_schemaVersion|int|The current schema version (3).|
|metadata_sensorId|string|UID of the Sumo Logic sensor used to ingest the log.|
|metadata_sensorInformation|map[string]string|(Deprecated) Information about the sensor used to ingest the log.|
|metadata_sensorZone|string|A name propagated from the sensors. In the case where sensors are installed in environments with overlapping IP address spaces, this is used to distinguish two identical IP addresses from each other.|
|metadata_sourceBlockId|string|The _blockId of the original source log message (from SumoLogic).|
|metadata_sourceCategory|string|The Sumologic source category of the data.|
|metadata_sourceMessageId|string|The _messageID of the original source log message (from SumoLogic CIP).|
|metadata_tenantId|string|(Deprecated) Unique identifier for the portal that data is being sent to.|
|metadata_vendor|string|The name of the company responsible for the data source.|
|month|int|Month pulled from the timestamp.|
|year|int|Year pulled from the timestamp.|


