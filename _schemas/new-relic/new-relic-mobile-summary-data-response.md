---
description: ''
layout: schema
name: MobileSummaryDataResponse
properties_list:
- description: ''
  name: active_users
  type: integer
- description: ''
  name: calls_per_session
  type: number
- description: ''
  name: failed_call_rate
  type: number
- description: ''
  name: interaction_time
  type: number
- description: ''
  name: launch_count
  type: integer
- description: ''
  name: remote_error_rate
  type: number
- description: ''
  name: response_time
  type: number
- description: ''
  name: throughput
  type: number
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-mobile-summary-data-response-schema.json
slug: new-relic-mobile-summary-data-response
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"active_users\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"calls_per_session\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"failed_call_rate\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 12.3\n    },\n    \"interaction_time\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"launch_count\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"remote_error_rate\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 12.3\n    },\n    \"response_time\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    },\n    \"throughput\": {\n      \"type\": \"number\",\n      \"format\": \"float\",\n      \"example\": 42.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"MobileSummaryDataResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-mobile-summary-data-response-schema.json
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
title: MobileSummaryDataResponse
---
