---
description: The attributes of a log event returned from the search API
layout: schema
name: LogAttributes
properties_list:
- description: ISO 8601 timestamp when the log was generated
  name: timestamp
  type: string
- description: The log level or severity status of the event
  name: status
  type: string
- description: The raw log message content
  name: message
  type: string
- description: The hostname of the machine that generated the log
  name: host
  type: string
- description: The name of the application or service that generated the log
  name: service
  type: string
- description: The technology source that generated the log (e.g., nginx, java)
  name: source
  type: string
- description: List of tags associated with the log event in key:value format
  name: tags
  type: array
- description: Custom key-value attributes extracted from the log message
  name: attributes
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-log-attributes-schema.json
slug: datadog-logs-log-attributes
source_filename: datadog-logs-log-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-log-attributes-schema.json\",\n  \"title\": \"LogAttributes\",\n  \"description\": \"The attributes of a log event returned from the search API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the log was generated\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The log level or severity status of the event\",\n      \"example\": \"OK\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The raw log message content\",\n      \"example\": \"CPU usage is high on {{host.name}}\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"\
  The hostname of the machine that generated the log\",\n      \"example\": \"example_value\"\n    },\n    \"service\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application or service that generated the log\",\n      \"example\": \"example_value\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"The technology source that generated the log (e.g., nginx, java)\",\n      \"example\": \"example_value\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"List of tags associated with the log event in key:value format\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Custom key-value attributes extracted from the log message\",\n      \"additionalProperties\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-log-attributes-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogAttributes
---
