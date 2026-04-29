---
description: A single metric data point
layout: schema
name: MetricDataPoint
properties_list:
- description: The metric name (e.g., cpu.usage.percent)
  name: name
  type: string
- description: The metric type
  name: type
  type: string
- description: The metric value. For gauge and count, a number. For summary, an object with count, sum, min, and max fields.
  name: value
  type: object
- description: Unix timestamp in milliseconds. Overrides the common timestamp for this metric.
  name: timestamp
  type: integer
- description: Measurement interval in milliseconds. Required for count and summary types.
  name: interval.ms
  type: integer
- description: Additional key-value attributes for this metric point
  name: attributes
  type: object
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-metric-metric-data-point-schema.json
slug: new-relic-metric-metric-data-point
source_filename: new-relic-metric-metric-data-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A single metric data point\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The metric name (e.g., cpu.usage.percent)\",\n      \"example\": \"example-resource-01\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The metric type\",\n      \"example\": \"gauge\",\n      \"enum\": [\n        \"gauge\",\n        \"count\",\n        \"summary\"\n      ]\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"description\": \"The metric value. For gauge and count, a number. For summary, an object with count, sum, min, and max fields.\",\n      \"example\": 42.5\n    },\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp in milliseconds. Overrides the common timestamp for this metric.\",\n      \"example\": 1718153645993\n    },\n    \"interval.ms\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"Measurement interval in milliseconds. Required for count and summary types.\",\n      \"example\": 100\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"description\": \"Additional key-value attributes for this metric point\",\n      \"example\": {\n        \"customAttribute\": \"example_value\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"value\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataPoint\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-metric-data-point-schema.json
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
title: MetricDataPoint
---
