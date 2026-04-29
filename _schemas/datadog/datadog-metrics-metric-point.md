---
description: A single data point consisting of a Unix timestamp and a numeric value
layout: schema
name: MetricPoint
properties_list:
- description: The Unix timestamp in seconds when this data point was recorded
  name: timestamp
  type: integer
- description: The numeric value of the metric at the given timestamp
  name: value
  type: number
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-point-schema.json
slug: datadog-metrics-metric-point
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-point-schema.json\",\n  \"title\": \"MetricPoint\",\n  \"description\": \"A single data point consisting of a Unix timestamp and a numeric value\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"The Unix timestamp in seconds when this data point was recorded\",\n      \"example\": 42\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"The numeric value of the metric at the given timestamp\",\n      \"example\": 95.5\n    }\n  },\n  \"required\": [\n    \"timestamp\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-point-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricPoint
---
