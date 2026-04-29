---
description: Schema for a Splunk event, the fundamental unit of data in Splunk. An event represents a single entry of machine data that has been indexed by Splunk, containing the raw event data along with metadata fields used for searching, filtering, and organizing data. Events are ingested through various data inputs including HTTP Event Collector (HEC), file monitors, TCP/UDP inputs, and scripted inputs.
layout: schema
name: Splunk Event
properties_list:
- description: The timestamp of the event. When submitting via HEC, this is epoch time in seconds. When retrieved from search results, the format depends on the output mode. If omitted during ingestion, Splunk assig
  name: time
  type: object
- description: The indexed timestamp of the event as stored in Splunk. This is the canonical time field used in search results and is always present on indexed events.
  name: _time
  type: string
- description: The original raw text of the event as it was received by Splunk. This contains the complete, unmodified event data before field extraction.
  name: _raw
  type: string
- description: 'The event payload when submitting via HTTP Event Collector. Can be a string for raw text events or a JSON object for structured events. This field is required when using the /services/collector/event '
  name: event
  type: object
- description: The hostname, IP address, or fully qualified domain name of the system that generated the event. This is a default metadata field that Splunk assigns during data ingestion.
  name: host
  type: string
- description: The source of the event data, typically a file path, network port, or data input name. Identifies where the data originated from on the host.
  name: source
  type: string
- description: The source type classifies the event data format and determines how Splunk parses and extracts fields. Splunk includes many built-in sourcetypes and custom ones can be defined.
  name: sourcetype
  type: string
- description: The name of the Splunk index where the event is stored. Indexes are the primary data repositories in Splunk.
  name: index
  type: string
- description: The time at which the event was indexed by Splunk, as opposed to when the event occurred. Stored as epoch time.
  name: _indextime
  type: string
- description: A sequence number assigned to the event within the search results. Used for ordering and pagination.
  name: _serial
  type: integer
- description: Internal Splunk field containing the bucket ID and offset for the event. Used for direct event access.
  name: _cd
  type: string
- description: The bucket ID where the event is stored within the index. Format is <index_name>~<bucket_id>~<guid>.
  name: _bkt
  type: string
- description: Server and index information as a two-element array containing the Splunk server name and the index name.
  name: _si
  type: array
- description: The number of lines in the raw event text
  name: linecount
  type: integer
- description: The name of the Splunk server that indexed this event. Relevant in distributed search environments.
  name: splunk_server
  type: string
- description: The server group of the Splunk server that indexed this event. Used in indexer clustering.
  name: splunk_server_group
  type: string
- description: The event type classification assigned by Splunk based on configured eventtype definitions.
  name: eventtype
  type: string
- description: Tags associated with the event based on field values and tag configurations.
  name: tag
  type: array
- description: Additional metadata fields to associate with the event during HEC ingestion. These are indexed as metadata and can be searched as indexed fields without being part of the raw event data.
  name: fields
  type: object
provider_name: Splunk
provider_slug: splunk
schema_file: json-schema/splunk-event-schema.json
slug: splunk-event
source_filename: splunk-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/splunk/blob/main/json-schema/splunk-event-schema.json\",\n  \"title\": \"Splunk Event\",\n  \"description\": \"Schema for a Splunk event, the fundamental unit of data in Splunk. An event represents a single entry of machine data that has been indexed by Splunk, containing the raw event data along with metadata fields used for searching, filtering, and organizing data. Events are ingested through various data inputs including HTTP Event Collector (HEC), file monitors, TCP/UDP inputs, and scripted inputs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"time\": {\n      \"oneOf\": [\n        {\n          \"type\": \"number\",\n          \"description\": \"Event timestamp as epoch time in seconds since 1970-01-01 00:00:00 UTC. Fractional seconds are supported for sub-second precision.\"\n        },\n        {\n          \"type\": \"string\",\n          \"\
  description\": \"Event timestamp as an ISO 8601 string or other Splunk-recognized time format.\"\n        }\n      ],\n      \"description\": \"The timestamp of the event. When submitting via HEC, this is epoch time in seconds. When retrieved from search results, the format depends on the output mode. If omitted during ingestion, Splunk assigns the current system time.\",\n      \"examples\": [\n        1704067200.000,\n        \"2024-01-01T00:00:00.000+00:00\"\n      ]\n    },\n    \"_time\": {\n      \"type\": \"string\",\n      \"description\": \"The indexed timestamp of the event as stored in Splunk. This is the canonical time field used in search results and is always present on indexed events.\",\n      \"examples\": [\n        \"2024-01-01T00:00:00.000+00:00\"\n      ]\n    },\n    \"_raw\": {\n      \"type\": \"string\",\n      \"description\": \"The original raw text of the event as it was received by Splunk. This contains the complete, unmodified event data before field extraction.\"\
  ,\n      \"examples\": [\n        \"2024-01-01 00:00:00 INFO  [main] - Application started successfully on port 8080\"\n      ]\n    },\n    \"event\": {\n      \"description\": \"The event payload when submitting via HTTP Event Collector. Can be a string for raw text events or a JSON object for structured events. This field is required when using the /services/collector/event endpoint.\",\n      \"oneOf\": [\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"object\",\n          \"additionalProperties\": true\n        }\n      ],\n      \"examples\": [\n        \"User authentication successful\",\n        {\n          \"message\": \"User logged in\",\n          \"user\": \"admin\",\n          \"action\": \"login\",\n          \"status\": \"success\"\n        }\n      ]\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname, IP address, or fully qualified domain name of the system that generated the event. This\
  \ is a default metadata field that Splunk assigns during data ingestion.\",\n      \"examples\": [\n        \"webserver01\",\n        \"10.0.1.100\",\n        \"app-server.example.com\"\n      ]\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The source of the event data, typically a file path, network port, or data input name. Identifies where the data originated from on the host.\",\n      \"examples\": [\n        \"/var/log/syslog\",\n        \"/var/log/apache2/access.log\",\n        \"udp:514\",\n        \"http:my_hec_token\"\n      ]\n    },\n    \"sourcetype\": {\n      \"type\": \"string\",\n      \"description\": \"The source type classifies the event data format and determines how Splunk parses and extracts fields. Splunk includes many built-in sourcetypes and custom ones can be defined.\",\n      \"examples\": [\n        \"syslog\",\n        \"access_combined\",\n        \"_json\",\n        \"splunkd\",\n        \"WinEventLog:Security\",\n  \
  \      \"aws:cloudtrail\"\n      ]\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the Splunk index where the event is stored. Indexes are the primary data repositories in Splunk.\",\n      \"default\": \"main\",\n      \"examples\": [\n        \"main\",\n        \"web_logs\",\n        \"security\",\n        \"_internal\",\n        \"_audit\"\n      ]\n    },\n    \"_indextime\": {\n      \"type\": \"string\",\n      \"description\": \"The time at which the event was indexed by Splunk, as opposed to when the event occurred. Stored as epoch time.\",\n      \"examples\": [\n        \"1704067210\"\n      ]\n    },\n    \"_serial\": {\n      \"type\": \"integer\",\n      \"description\": \"A sequence number assigned to the event within the search results. Used for ordering and pagination.\",\n      \"minimum\": 0\n    },\n    \"_cd\": {\n      \"type\": \"string\",\n      \"description\": \"Internal Splunk field containing the bucket ID and offset\
  \ for the event. Used for direct event access.\",\n      \"examples\": [\n        \"1:234567\"\n      ]\n    },\n    \"_bkt\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket ID where the event is stored within the index. Format is <index_name>~<bucket_id>~<guid>.\",\n      \"examples\": [\n        \"main~1~A1B2C3D4-E5F6-7890-ABCD-EF1234567890\"\n      ]\n    },\n    \"_si\": {\n      \"type\": \"array\",\n      \"description\": \"Server and index information as a two-element array containing the Splunk server name and the index name.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"minItems\": 2,\n      \"maxItems\": 2,\n      \"examples\": [\n        [\"splunk-server\", \"main\"]\n      ]\n    },\n    \"linecount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of lines in the raw event text\",\n      \"minimum\": 1\n    },\n    \"splunk_server\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the\
  \ Splunk server that indexed this event. Relevant in distributed search environments.\",\n      \"examples\": [\n        \"idx01.example.com\"\n      ]\n    },\n    \"splunk_server_group\": {\n      \"type\": \"string\",\n      \"description\": \"The server group of the Splunk server that indexed this event. Used in indexer clustering.\"\n    },\n    \"eventtype\": {\n      \"type\": \"string\",\n      \"description\": \"The event type classification assigned by Splunk based on configured eventtype definitions.\"\n    },\n    \"tag\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the event based on field values and tag configurations.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"fields\": {\n      \"type\": \"object\",\n      \"description\": \"Additional metadata fields to associate with the event during HEC ingestion. These are indexed as metadata and can be searched as indexed fields without being part of the raw event data.\"\
  ,\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          },\n          {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        ]\n      },\n      \"examples\": [\n        {\n          \"environment\": \"production\",\n          \"region\": \"us-west-2\",\n          \"severity\": \"info\"\n        }\n      ]\n    }\n  },\n  \"if\": {\n    \"required\": [\"event\"]\n  },\n  \"then\": {\n    \"description\": \"When the event field is present (HEC submission format), the event field is required.\"\n  },\n  \"else\": {\n    \"description\": \"When the event field is absent (search result format), _time and _raw are the core fields.\"\n  },\n  \"examples\": [\n    {\n      \"time\": 1704067200.000,\n      \"host\": \"webserver01\",\n\
  \      \"source\": \"/var/log/apache2/access.log\",\n      \"sourcetype\": \"access_combined\",\n      \"index\": \"web_logs\",\n      \"event\": \"192.168.1.100 - admin [01/Jan/2024:00:00:00 +0000] \\\"GET /api/v1/status HTTP/1.1\\\" 200 1234\"\n    },\n    {\n      \"_time\": \"2024-01-01T00:00:00.000+00:00\",\n      \"_raw\": \"2024-01-01 00:00:00 INFO  [main] - Application started successfully on port 8080\",\n      \"host\": \"app-server.example.com\",\n      \"source\": \"/var/log/application.log\",\n      \"sourcetype\": \"_json\",\n      \"index\": \"main\",\n      \"linecount\": 1,\n      \"splunk_server\": \"idx01.example.com\"\n    },\n    {\n      \"time\": 1704067200.000,\n      \"host\": \"sensor-gateway\",\n      \"source\": \"iot:telemetry\",\n      \"sourcetype\": \"_json\",\n      \"index\": \"iot_data\",\n      \"event\": {\n        \"device_id\": \"sensor-001\",\n        \"temperature\": 22.5,\n        \"humidity\": 45.2,\n        \"location\": \"building-a\"\n    \
  \  },\n      \"fields\": {\n        \"environment\": \"production\",\n        \"region\": \"us-west-2\"\n      }\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/splunk/refs/heads/main/json-schema/splunk-event-schema.json
tags:
- Analytics
- Data Analysis
- Logging
- Machine Data
- Monitoring
- Observability
- Platform
- Security
- SIEM
title: Splunk Event
---
