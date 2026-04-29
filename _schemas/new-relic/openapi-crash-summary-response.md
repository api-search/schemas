---
description: CrashSummaryResponse schema
layout: schema
name: CrashSummaryResponse
properties_list:
- description: ''
  name: crash_count
  type: integer
- description: ''
  name: crash_rate
  type: number
- description: ''
  name: supports_crash_data
  type: boolean
- description: ''
  name: unresolved_crash_count
  type: integer
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-crash-summary-response-schema.json
slug: openapi-crash-summary-response
source_filename: openapi-crash-summary-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-crash-summary-response-schema.json\",\n  \"title\": \"CrashSummaryResponse\",\n  \"description\": \"CrashSummaryResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"crash_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"crash_rate\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 12.3\n    },\n    \"supports_crash_data\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"unresolved_crash_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-crash-summary-response-schema.json
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
title: CrashSummaryResponse
---
