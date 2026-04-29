---
description: ''
layout: schema
name: MetricListResponse
properties_list:
- description: ''
  name: metrics
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-metric-list-response-schema.json
slug: new-relic-metric-list-response
source_filename: new-relic-metric-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"values\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"example-resource-01\"\n          },\n          \"values\": {\n            \"type\": \"array\",\n            \"example\": [\n              \"example_string\"\n            ],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricListResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-list-response-schema.json
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
title: MetricListResponse
---
