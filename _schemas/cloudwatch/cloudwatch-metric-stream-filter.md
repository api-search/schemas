---
description: Contains the configuration for a metric stream filter.
layout: schema
name: MetricStreamFilter
properties_list:
- description: The name of the metric namespace in the filter.
  name: Namespace
  type: string
- description: The names of the metrics to either include or exclude from the metric stream.
  name: MetricNames
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-stream-filter-schema.json
slug: cloudwatch-metric-stream-filter
source_filename: cloudwatch-metric-stream-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricStreamFilter\",\n  \"type\": \"object\",\n  \"description\": \"Contains the configuration for a metric stream filter.\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric namespace in the filter.\"\n    },\n    \"MetricNames\": {\n      \"type\": \"array\",\n      \"description\": \"The names of the metrics to either include or exclude from the metric stream.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-stream-filter-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricStreamFilter
---
