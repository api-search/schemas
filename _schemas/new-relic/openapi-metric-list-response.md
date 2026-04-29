---
description: MetricListResponse schema
layout: schema
name: MetricListResponse
properties_list:
- description: ''
  name: metrics
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-metric-list-response-schema.json
slug: openapi-metric-list-response
source_filename: openapi-metric-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-list-response-schema.json\",\n  \"title\": \"MetricListResponse\",\n  \"description\": \"MetricListResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricParserResponseType\"\n      },\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"values\": [\n            {}\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-list-response-schema.json
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
