---
description: AppSummaryDataResponse schema
layout: schema
name: AppSummaryDataResponse
properties_list:
- description: ''
  name: apdex_score
  type: number
- description: ''
  name: error_rate
  type: number
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
schema_file: json-schema/openapi-app-summary-data-response-schema.json
slug: openapi-app-summary-data-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-summary-data-response-schema.json\",\n  \"title\": \"AppSummaryDataResponse\",\n  \"description\": \"AppSummaryDataResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apdex_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 87.5\n    },\n    \"error_rate\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 12.3\n    },\n    \"instance_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"response_time\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-app-summary-data-response-schema.json
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
title: AppSummaryDataResponse
---
