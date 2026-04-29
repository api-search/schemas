---
description: ''
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
schema_file: json-schema/new-relic-label-origins-response-schema.json
slug: new-relic-label-origins-response
source_filename: new-relic-label-origins-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"agents\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"apm\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    },\n    \"synthetics\": {\n      \"type\": \"array\",\n      \"example\": [\n        100\n      ],\n      \"items\": {\n        \"type\": \"integer\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LabelOriginsResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-label-origins-response-schema.json
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
