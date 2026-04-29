---
description: The result of a log export operation, containing a page of records.
layout: schema
name: LogExportResult
properties_list:
- description: Cursor for the next page of export results.
  name: nextSliceKey
  type: string
- description: The list of exported log records on this page.
  name: results
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/log-monitoring-api-v2-log-export-result-schema.json
slug: log-monitoring-api-v2-log-export-result
source_filename: log-monitoring-api-v2-log-export-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-export-result-schema.json\",\n  \"title\": \"LogExportResult\",\n  \"description\": \"The result of a log export operation, containing a page of records.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"nextSliceKey\": {\n      \"type\": \"string\",\n      \"description\": \"Cursor for the next page of export results.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The list of exported log records on this page.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LogRecord\"\n      },\n      \"example\": [\n        {\n          \"timestamp\": \"example-value\",\n          \"content\": \"example-value\",\n          \"severity\": \"HIGH\",\n          \"log.source\"\
  : \"example-value\",\n          \"dt.entity.host\": \"example-value\",\n          \"additionalFields\": {}\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/log-monitoring-api-v2-log-export-result-schema.json
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
title: LogExportResult
---
