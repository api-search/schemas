---
description: EndUserSummaryDataResponse schema
layout: schema
name: EndUserSummaryDataResponse
properties_list:
- description: ''
  name: apdex_score
  type: number
- description: ''
  name: response_time
  type: number
- description: ''
  name: throughput
  type: number
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-end-user-summary-data-response-schema.json
slug: openapi-end-user-summary-data-response
source_filename: openapi-end-user-summary-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-end-user-summary-data-response-schema.json\",\n  \"title\": \"EndUserSummaryDataResponse\",\n  \"description\": \"EndUserSummaryDataResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"apdex_score\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 87.5\n    },\n    \"response_time\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-end-user-summary-data-response-schema.json
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
title: EndUserSummaryDataResponse
---
