---
description: The result of a log search query.
layout: schema
name: LogRecordSearchResult
properties_list:
- description: The cursor for the next page of results. Null if all results have been returned.
  name: nextSliceKey
  type: string
- description: The list of log records matching the search query on this page.
  name: results
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-log-monitoring-v2-log-record-search-result-schema.json
slug: dynatrace-log-monitoring-v2-log-record-search-result
source_filename: dynatrace-log-monitoring-v2-log-record-search-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a log search query.\",\n  \"properties\": {\n    \"nextSliceKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results. Null if all results have been returned.\",\n      \"example\": \"example-value\"\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"The list of log records matching the search query on this page.\",\n      \"example\": [\n        {\n          \"timestamp\": \"example-value\",\n          \"content\": \"example-value\",\n          \"severity\": \"HIGH\",\n          \"log.source\": \"example-value\",\n          \"dt.entity.host\": \"example-value\",\n          \"additionalFields\": {}\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A log record retrieved from the Dynatrace Grail data lakehouse. Contains the original log content plus enriched metadata added by Dynatrace during\
  \ ingestion and processing.\",\n        \"properties\": {\n          \"timestamp\": {\n            \"type\": \"string\",\n            \"description\": \"The timestamp of the log record in ISO 8601 format.\",\n            \"example\": \"example-value\"\n          },\n          \"content\": {\n            \"type\": \"string\",\n            \"description\": \"The log message content.\",\n            \"example\": \"example-value\"\n          },\n          \"severity\": {\n            \"type\": \"string\",\n            \"description\": \"The severity level of the log record.\",\n            \"example\": \"HIGH\"\n          },\n          \"log.source\": {\n            \"type\": \"string\",\n            \"description\": \"The source identifier of the log record.\",\n            \"example\": \"example-value\"\n          },\n          \"dt.entity.host\": {\n            \"type\": \"string\",\n            \"description\": \"The associated host entity ID.\",\n            \"example\": \"example-value\"\
  \n          },\n          \"additionalFields\": {\n            \"type\": \"object\",\n            \"description\": \"Additional fields present in the log record beyond the standard set. Content varies based on what was ingested and how OpenPipeline processed the record.\",\n            \"example\": {}\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LogRecordSearchResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-log-monitoring-v2-log-record-search-result-schema.json
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
title: LogRecordSearchResult
---
