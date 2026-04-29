---
description: A single log record
layout: schema
name: LogRecord
properties_list:
- description: Unix epoch timestamp in milliseconds when the log event occurred
  name: timestamp
  type: integer
- description: The log message text
  name: message
  type: string
- description: Log severity level
  name: level
  type: string
- description: Log format type for automatic parsing (e.g., nginx, apache, syslog)
  name: logtype
  type: string
- description: Additional key-value attributes for this log record
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/log-api-log-record-schema.json
slug: log-api-log-record
source_filename: log-api-log-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-record-schema.json\",\n  \"title\": \"LogRecord\",\n  \"description\": \"A single log record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix epoch timestamp in milliseconds when the log event occurred\",\n      \"example\": 1718153645993\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The log message text\",\n      \"maxLength\": 32768,\n      \"example\": \"Operation completed successfully\"\n    },\n    \"level\": {\n      \"type\": \"string\",\n      \"description\": \"Log severity level\",\n      \"enum\": [\n        \"FATAL\",\n        \"ERROR\",\n        \"WARN\",\n        \"WARNING\",\n        \"INFO\",\n        \"DEBUG\",\n        \"TRACE\"\n      ],\n      \"example\": \"\
  FATAL\"\n    },\n    \"logtype\": {\n      \"type\": \"string\",\n      \"description\": \"Log format type for automatic parsing (e.g., nginx, apache, syslog)\",\n      \"example\": \"standard\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key-value attributes for this log record\",\n      \"additionalProperties\": {\n        \"oneOf\": [\n          {\n            \"type\": \"string\"\n          },\n          {\n            \"type\": \"number\"\n          },\n          {\n            \"type\": \"boolean\"\n          }\n        ]\n      },\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  },\n  \"additionalProperties\": {\n    \"description\": \"Additional top-level attributes are accepted and stored\"\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/log-api-log-record-schema.json
tags:
- Analysis
- Analytics
- APM
- DevOps
- Infrastructure
- Monitoring
- Observability
- Performance
- Platform
title: LogRecord
---
