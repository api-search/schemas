---
description: Filter criteria for log search queries
layout: schema
name: LogsQueryFilter
properties_list:
- description: A Datadog log search query string to filter log events (e.g., service:web status:error)
  name: query
  type: string
- description: List of log index names to search; if empty, all indexes are searched
  name: indexes
  type: array
- description: The start of the time range for the search in ISO 8601 format or relative format (e.g., now-15m)
  name: from
  type: string
- description: The end of the time range for the search in ISO 8601 format or relative format (e.g., now)
  name: to
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-query-filter-schema.json
slug: datadog-logs-logs-query-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-query-filter-schema.json\",\n  \"title\": \"LogsQueryFilter\",\n  \"description\": \"Filter criteria for log search queries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"A Datadog log search query string to filter log events (e.g., service:web status:error)\",\n      \"example\": \"avg:system.cpu.user{*}\"\n    },\n    \"indexes\": {\n      \"type\": \"array\",\n      \"description\": \"List of log index names to search; if empty, all indexes are searched\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"The start of the time range for the search in ISO 8601 format or relative format (e.g., now-15m)\",\n      \"example\": \"example_value\"\
  \n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"The end of the time range for the search in ISO 8601 format or relative format (e.g., now)\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-query-filter-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsQueryFilter
---
