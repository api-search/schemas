---
description: Response time metrics for a monitor.
layout: schema
name: ResponseTimesResponse
properties_list:
- description: Array of response time data points.
  name: data
  type: array
provider_name: Better Stack
provider_slug: better-stack
schema_file: json-schema/better-stack-response-times-response-schema.json
slug: better-stack-response-times-response
source_filename: better-stack-response-times-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-response-times-response-schema.json\",\n  \"title\": \"ResponseTimesResponse\",\n  \"description\": \"Response time metrics for a monitor.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of response time data points.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"at\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Timestamp of the measurement.\",\n            \"example\": \"2026-04-19T10:00:00Z\"\n          },\n          \"response_time\": {\n            \"type\": \"integer\",\n            \"description\": \"Response time in milliseconds.\",\n            \"example\": 142\n          },\n          \"region\":\
  \ {\n            \"type\": \"string\",\n            \"description\": \"Region where the check was performed.\",\n            \"example\": \"us\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/better-stack/refs/heads/main/json-schema/better-stack-response-times-response-schema.json
tags:
- Incidents
- Logs
- Monitoring
- Platform
- Status
- Uptime
- Observability
- On-Call
- Heartbeats
title: ResponseTimesResponse
---
