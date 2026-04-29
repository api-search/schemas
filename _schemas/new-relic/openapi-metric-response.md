---
description: MetricResponse schema
layout: schema
name: MetricResponse
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: timeslices
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-metric-response-schema.json
slug: openapi-metric-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-response-schema.json\",\n  \"title\": \"MetricResponse\",\n  \"description\": \"MetricResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"example-resource-01\"\n    },\n    \"timeslices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TimesliceResponse\"\n      },\n      \"example\": [\n        {\n          \"from\": \"2026-04-18T14:30:00Z\",\n          \"to\": \"2026-04-18T14:30:00Z\",\n          \"values\": {}\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-response-schema.json
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
title: MetricResponse
---
