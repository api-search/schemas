---
description: ''
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
schema_file: json-schema/new-relic-metric-data-response-type-schema.json
slug: new-relic-metric-data-response-type
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"from\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"timeslices\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"example-resource-01\"\n          },\n          \"timeslices\": {\n            \"type\": \"array\",\n            \"example\": [\n              {\n                \"from\": \"2026-04-18T14:30:00Z\",\n                \"to\": \"2026-04-18T14:30:00Z\",\n                \"values\": {}\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"from\": {\n\
  \                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"example\": \"2026-04-18T14:30:00Z\"\n                },\n                \"to\": {\n                  \"type\": \"string\",\n                  \"format\": \"date-time\",\n                  \"example\": \"2026-04-18T14:30:00Z\"\n                },\n                \"values\": {\n                  \"type\": \"object\",\n                  \"example\": {},\n                  \"properties\": {}\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"metrics_found\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"metrics_not_found\": {\n      \"type\": \"string\",\n      \"example\": \"example_string\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"MetricDataResponseType\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-data-response-type-schema.json
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
