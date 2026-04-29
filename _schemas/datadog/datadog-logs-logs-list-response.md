---
description: Response containing matching log events from a search query
layout: schema
name: LogsListResponse
properties_list:
- description: List of matching log events
  name: data
  type: array
- description: Metadata about the search response including pagination information
  name: meta
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-list-response-schema.json
slug: datadog-logs-logs-list-response
source_filename: datadog-logs-logs-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-list-response-schema.json\",\n  \"title\": \"LogsListResponse\",\n  \"description\": \"Response containing matching log events from a search query\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"List of matching log events\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Log\"\n      }\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the search response including pagination information\",\n      \"properties\": {\n        \"page\": {\n          \"type\": \"object\",\n          \"description\": \"Pagination details for continuing the search\",\n          \"properties\": {\n            \"after\": {\n              \"type\": \"string\",\n              \"description\"\
  : \"Cursor token to retrieve the next page of results\"\n            }\n          }\n        },\n        \"elapsed\": {\n          \"type\": \"integer\",\n          \"description\": \"Time in milliseconds taken to execute the search query\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"Status of the search request (done, timeout)\",\n          \"enum\": [\n            \"done\",\n            \"timeout\"\n          ]\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-list-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsListResponse
---
