---
description: Array of log data batch objects
layout: schema
name: LogPayload
properties_list: []
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-log-log-payload-schema.json
slug: new-relic-log-log-payload
source_filename: new-relic-log-log-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"array\",\n  \"description\": \"Array of log data batch objects\",\n  \"items\": {\n    \"type\": \"object\",\n    \"description\": \"A batch of log records with optional shared attributes\",\n    \"properties\": {\n      \"common\": {\n        \"type\": \"object\",\n        \"description\": \"Shared attributes applied to all log records in this batch\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"integer\",\n            \"description\": \"Default Unix timestamp in milliseconds for all logs in the batch\",\n            \"example\": 1718153645993\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"description\": \"Key-value attributes applied to all logs in this batch\",\n            \"example\": {\n              \"customAttribute\": \"example_value\"\n            }\n          }\n        }\n      },\n      \"logs\": {\n        \"type\": \"array\",\n        \"description\": \"Array of\
  \ individual log records\",\n        \"example\": [\n          {\n            \"timestamp\": 1718153645993,\n            \"message\": \"Operation completed successfully\",\n            \"level\": \"FATAL\",\n            \"logtype\": \"standard\",\n            \"attributes\": {\n              \"customAttribute\": \"example_value\"\n            }\n          }\n        ],\n        \"items\": {\n          \"type\": \"object\",\n          \"description\": \"A single log record\",\n          \"properties\": {\n            \"timestamp\": {\n              \"type\": \"integer\",\n              \"description\": \"Unix epoch timestamp in milliseconds when the log event occurred\",\n              \"example\": 1718153645993\n            },\n            \"message\": {\n              \"type\": \"string\",\n              \"description\": \"The log message text\",\n              \"example\": \"Operation completed successfully\"\n            },\n            \"level\": {\n              \"type\": \"string\"\
  ,\n              \"description\": \"Log severity level\",\n              \"example\": \"FATAL\",\n              \"enum\": [\n                \"FATAL\",\n                \"ERROR\",\n                \"WARN\",\n                \"WARNING\",\n                \"INFO\",\n                \"DEBUG\",\n                \"TRACE\"\n              ]\n            },\n            \"logtype\": {\n              \"type\": \"string\",\n              \"description\": \"Log format type for automatic parsing (e.g., nginx, apache, syslog)\",\n              \"example\": \"standard\"\n            },\n            \"attributes\": {\n              \"type\": \"object\",\n              \"description\": \"Additional key-value attributes for this log record\",\n              \"example\": {\n                \"customAttribute\": \"example_value\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"required\": [\n      \"logs\"\n    ]\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"LogPayload\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-log-log-payload-schema.json
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
title: LogPayload
---
