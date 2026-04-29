---
description: Request body for searching log events
layout: schema
name: LogsListRequest
properties_list:
- description: ''
  name: filter
  type: object
- description: The sort order for log results, either ascending or descending by timestamp
  name: sort
  type: string
- description: Pagination configuration for log search results
  name: page
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-list-request-schema.json
slug: datadog-logs-logs-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-list-request-schema.json\",\n  \"title\": \"LogsListRequest\",\n  \"description\": \"Request body for searching log events\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filter\": {\n      \"$ref\": \"#/components/schemas/LogsQueryFilter\"\n    },\n    \"sort\": {\n      \"type\": \"string\",\n      \"description\": \"The sort order for log results, either ascending or descending by timestamp\",\n      \"enum\": [\n        \"timestamp\",\n        \"-timestamp\"\n      ],\n      \"example\": \"timestamp\"\n    },\n    \"page\": {\n      \"type\": \"object\",\n      \"description\": \"Pagination configuration for log search results\",\n      \"properties\": {\n        \"cursor\": {\n          \"type\": \"string\",\n          \"description\": \"A cursor token from a previous response to\
  \ retrieve the next page of results\"\n        },\n        \"limit\": {\n          \"type\": \"integer\",\n          \"description\": \"The maximum number of logs to return per page (default 10, max 1000)\",\n          \"minimum\": 1,\n          \"maximum\": 1000,\n          \"default\": 10\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-list-request-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsListRequest
---
