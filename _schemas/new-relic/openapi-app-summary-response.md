---
description: AppSummaryResponse schema
layout: schema
name: AppSummaryResponse
properties_list:
- description: ''
  name: apdex_score
  type: number
- description: ''
  name: apdex_target
  type: number
- description: ''
  name: concurrent_instance_count
  type: integer
- description: ''
  name: error_rate
  type: number
- description: ''
  name: host_count
  type: integer
- description: ''
  name: instance_count
  type: integer
- description: ''
  name: response_time
  type: number
- description: ''
  name: throughput
  type: number
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-app-summary-response-schema.json
slug: openapi-app-summary-response
source_filename: openapi-app-summary-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-summary-response-schema.json\",\n  \"title\": \"AppSummaryResponse\",\n  \"description\": \"AppSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apdex_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 87.5\n    },\n    \"apdex_target\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"concurrent_instance_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"error_rate\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 12.3\n    },\n    \"host_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"instance_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"response_time\"\
  : {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-summary-response-schema.json
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
title: AppSummaryResponse
---
