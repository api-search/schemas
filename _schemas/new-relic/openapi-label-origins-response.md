---
description: LabelOriginsResponse schema
layout: schema
name: LabelOriginsResponse
properties_list:
- description: ''
  name: agents
  type: array
- description: ''
  name: apm
  type: array
- description: ''
  name: synthetics
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-label-origins-response-schema.json
slug: openapi-label-origins-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-origins-response-schema.json\",\n  \"title\": \"LabelOriginsResponse\",\n  \"description\": \"LabelOriginsResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"agents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    },\n    \"apm\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    },\n    \"synthetics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n      },\n      \"example\": [\n        100\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-label-origins-response-schema.json
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
title: LabelOriginsResponse
---
