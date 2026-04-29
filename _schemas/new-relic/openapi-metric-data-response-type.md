---
description: MetricDataResponseType schema
layout: schema
name: MetricDataResponseType
properties_list:
- description: ''
  name: from
  type: string
- description: ''
  name: metrics
  type: array
- description: ''
  name: metrics_found
  type: string
- description: ''
  name: metrics_not_found
  type: string
- description: ''
  name: to
  type: string
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/openapi-metric-data-response-type-schema.json
slug: openapi-metric-data-response-type
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-data-response-type-schema.json\",\n  \"title\": \"MetricDataResponseType\",\n  \"description\": \"MetricDataResponseType schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricResponse\"\n      },\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"timeslices\": [\n            {}\n          ]\n        }\n      ]\n    },\n    \"metrics_found\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"metrics_not_found\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\
  \n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/openapi-metric-data-response-type-schema.json
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
title: MetricDataResponseType
---
