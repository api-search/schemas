---
description: A log record retrieved from the Dynatrace Grail data lakehouse. Contains the original log content plus enriched metadata added by Dynatrace during ingestion and processing.
layout: schema
name: LogRecord
properties_list:
- description: The timestamp of the log record in ISO 8601 format.
  name: timestamp
  type: string
- description: The log message content.
  name: content
  type: string
- description: The severity level of the log record.
  name: severity
  type: string
- description: The source identifier of the log record.
  name: log.source
  type: string
- description: The associated host entity ID.
  name: dt.entity.host
  type: string
- description: Additional fields present in the log record beyond the standard set. Content varies based on what was ingested and how OpenPipeline processed the record.
  name: additionalFields
  type: object
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-log-monitoring-v2-log-record-schema.json
slug: dynatrace-log-monitoring-v2-log-record
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A log record retrieved from the Dynatrace Grail data lakehouse. Contains the original log content plus enriched metadata added by Dynatrace during ingestion and processing.\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the log record in ISO 8601 format.\",\n      \"example\": \"example-value\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The log message content.\",\n      \"example\": \"example-value\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the log record.\",\n      \"example\": \"HIGH\"\n    },\n    \"log.source\": {\n      \"type\": \"string\",\n      \"description\": \"The source identifier of the log record.\",\n      \"example\": \"example-value\"\n    },\n    \"dt.entity.host\": {\n      \"type\": \"string\",\n      \"description\": \"The associated\
  \ host entity ID.\",\n      \"example\": \"example-value\"\n    },\n    \"additionalFields\": {\n      \"type\": \"object\",\n      \"description\": \"Additional fields present in the log record beyond the standard set. Content varies based on what was ingested and how OpenPipeline processed the record.\",\n      \"example\": {}\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogRecord\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-log-monitoring-v2-log-record-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: LogRecord
---
