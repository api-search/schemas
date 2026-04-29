---
description: Represents a specific metric.
layout: schema
name: Metric
properties_list:
- description: The namespace of the metric.
  name: Namespace
  type: string
- description: The name of the metric.
  name: MetricName
  type: string
- description: The dimensions for the metric.
  name: Dimensions
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-schema.json
slug: cloudwatch-metric
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metric\",\n  \"type\": \"object\",\n  \"description\": \"Represents a specific metric.\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions for the metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Metric
---
