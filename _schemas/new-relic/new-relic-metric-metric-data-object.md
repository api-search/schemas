---
description: A container for a batch of metrics with optional shared attributes
layout: schema
name: MetricDataObject
properties_list:
- description: Shared attributes applied to all metrics in this data object unless overridden at the metric level
  name: common
  type: object
- description: Array of individual metric data points
  name: metrics
  type: array
provider_name: New Relic
provider_slug: new-relic
schema_file: json-schema/new-relic-metric-metric-data-object-schema.json
slug: new-relic-metric-metric-data-object
source_filename: new-relic-metric-metric-data-object-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"A container for a batch of metrics with optional shared attributes\",\n  \"properties\": {\n    \"common\": {\n      \"type\": \"object\",\n      \"description\": \"Shared attributes applied to all metrics in this data object unless overridden at the metric level\",\n      \"properties\": {\n        \"timestamp\": {\n          \"type\": \"integer\",\n          \"description\": \"Unix timestamp in milliseconds for all metrics in this batch\",\n          \"example\": 1718153645993\n        },\n        \"interval.ms\": {\n          \"type\": \"integer\",\n          \"description\": \"Default measurement interval in milliseconds for count and summary metrics\",\n          \"example\": 100\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value pairs applied to all metrics in the batch. Values can be strings, numbers, or booleans.\",\n          \"example\": {\n            \"\
  customAttribute\": \"example_value\"\n          }\n        }\n      }\n    },\n    \"metrics\": {\n      \"type\": \"array\",\n      \"description\": \"Array of individual metric data points\",\n      \"example\": [\n        {\n          \"name\": \"example-resource-01\",\n          \"type\": \"gauge\",\n          \"value\": 42.5,\n          \"timestamp\": 1718153645993,\n          \"interval.ms\": 100,\n          \"attributes\": {\n            \"customAttribute\": \"example_value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A single metric data point\",\n        \"properties\": {\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The metric name (e.g., cpu.usage.percent)\",\n            \"example\": \"example-resource-01\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"description\": \"The metric type\",\n            \"example\": \"gauge\"\
  ,\n            \"enum\": [\n              \"gauge\",\n              \"count\",\n              \"summary\"\n            ]\n          },\n          \"value\": {\n            \"type\": \"object\",\n            \"description\": \"The metric value. For gauge and count, a number. For summary, an object with count, sum, min, and max fields.\",\n            \"example\": 42.5\n          },\n          \"timestamp\": {\n            \"type\": \"integer\",\n            \"description\": \"Unix timestamp in milliseconds. Overrides the common timestamp for this metric.\",\n            \"example\": 1718153645993\n          },\n          \"interval.ms\": {\n            \"type\": \"integer\",\n            \"description\": \"Measurement interval in milliseconds. Required for count and summary types.\",\n            \"example\": 100\n          },\n          \"attributes\": {\n            \"type\": \"object\",\n            \"description\": \"Additional key-value attributes for this metric point\",\n       \
  \     \"example\": {\n              \"customAttribute\": \"example_value\"\n            }\n          }\n        },\n        \"required\": [\n          \"name\",\n          \"type\",\n          \"value\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"metrics\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataObject\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/new-relic/refs/heads/main/json-schema/new-relic-metric-metric-data-object-schema.json
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
