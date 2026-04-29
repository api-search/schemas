---
description: A container for a batch of metrics with optional shared attributes
layout: schema
name: MetricDataObject
properties_list:
- description: ''
  name: common
  type: object
- description: Array of individual metric data points
  name: metrics
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/metric-api-metric-data-object-schema.json
slug: metric-api-metric-data-object
source_filename: metric-api-metric-data-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-metric-data-object-schema.json\",\n  \"title\": \"MetricDataObject\",\n  \"description\": \"A container for a batch of metrics with optional shared attributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"common\": {\n      \"$ref\": \"#/components/schemas/CommonBlock\"\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"Array of individual metric data points\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricDataPoint\"\n      },\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"type\": \"gauge\",\n          \"value\": 42.5,\n          \"timestamp\": 1718153645993,\n          \"interval.ms\": 100,\n          \"attributes\": {\n            \"customAttribute\": \"example_value\"\n          }\n    \
  \    }\n      ]\n    }\n  },\n  \"required\": [\n    \"metrics\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/metric-api-metric-data-object-schema.json
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
title: MetricDataObject
---
