---
description: A single log entry for the Azure Log Analytics Ingestion API. The schema must match the stream declaration in the data collection rule.
layout: schema
name: LogEntry
properties_list:
- description: The timestamp of the log entry.
  name: TimeGenerated
  type: string
- description: The computer or source generating the log.
  name: Computer
  type: string
- description: Additional context or message for the log entry.
  name: AdditionalContext
  type: string
provider_name: Azure Log Analytics
provider_slug: azure-log-analytics
schema_file: json-schema/ingestion-api-log-entry-schema.json
slug: ingestion-api-log-entry
source_filename: ingestion-api-log-entry-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/ingestion-api-log-entry-schema.json\",\n  \"title\": \"LogEntry\",\n  \"description\": \"A single log entry for the Azure Log Analytics Ingestion API. The schema must match the stream declaration in the data collection rule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TimeGenerated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp of the log entry.\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"Computer\": {\n      \"type\": \"string\",\n      \"description\": \"The computer or source generating the log.\",\n      \"example\": \"web-server-01\"\n    },\n    \"AdditionalContext\": {\n      \"type\": \"string\",\n      \"description\": \"Additional context or message for the log entry.\",\n      \"example\": \"Application\
  \ startup complete\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-log-analytics/refs/heads/main/json-schema/ingestion-api-log-entry-schema.json
tags:
- Analytics
- Azure
- Cloud
- Logging
- Monitoring
title: LogEntry
---
