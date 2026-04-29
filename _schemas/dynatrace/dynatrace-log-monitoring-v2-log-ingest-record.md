---
description: A single log record to ingest into the Dynatrace Grail data lakehouse. The content field is required. Additional fields provide context for routing, filtering, and entity association.
layout: schema
name: LogIngestRecord
properties_list:
- description: The main log message or text. Required. This is the primary searchable content of the log record.
  name: content
  type: string
- description: The severity level of the log record. Standard syslog severity levels are supported.
  name: severity
  type: string
- description: The timestamp of the log record. Accepts ISO 8601 format (e.g., 2024-01-15T10:30:00.000Z) or Unix timestamp in milliseconds. If not specified, the ingestion time is used.
  name: timestamp
  type: string
- description: A string identifier for the source of the log record, such as an application name, component, or log file path.
  name: log.source
  type: string
- description: The Dynatrace host entity ID to associate this log record with, e.g., HOST-1234567890ABCDEF. This enables correlation between logs and monitored infrastructure.
  name: dt.entity.host
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-log-monitoring-v2-log-ingest-record-schema.json
slug: dynatrace-log-monitoring-v2-log-ingest-record
source_filename: dynatrace-log-monitoring-v2-log-ingest-record-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single log record to ingest into the Dynatrace Grail data lakehouse. The content field is required. Additional fields provide context for routing, filtering, and entity association.\",\n  \"properties\": {\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"The main log message or text. Required. This is the primary searchable content of the log record.\",\n      \"example\": \"example-value\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"The severity level of the log record. Standard syslog severity levels are supported.\",\n      \"example\": \"EMERGENCY\",\n      \"enum\": [\n        \"EMERGENCY\",\n        \"ALERT\",\n        \"CRITICAL\",\n        \"ERROR\",\n        \"WARNING\",\n        \"NOTICE\",\n        \"INFO\",\n        \"DEBUG\",\n        \"TRACE\"\n      ]\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp\
  \ of the log record. Accepts ISO 8601 format (e.g., 2024-01-15T10:30:00.000Z) or Unix timestamp in milliseconds. If not specified, the ingestion time is used.\",\n      \"example\": \"example-value\"\n    },\n    \"log.source\": {\n      \"type\": \"string\",\n      \"description\": \"A string identifier for the source of the log record, such as an application name, component, or log file path.\",\n      \"example\": \"example-value\"\n    },\n    \"dt.entity.host\": {\n      \"type\": \"string\",\n      \"description\": \"The Dynatrace host entity ID to associate this log record with, e.g., HOST-1234567890ABCDEF. This enables correlation between logs and monitored infrastructure.\",\n      \"example\": \"example-value\"\n    }\n  },\n  \"required\": [\n    \"content\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogIngestRecord\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-log-monitoring-v2-log-ingest-record-schema.json
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
title: LogIngestRecord
---
