---
description: ''
layout: schema
name: GetMetricStatisticsOutput
properties_list:
- description: A label for the specified metric.
  name: Label
  type: string
- description: The data points for the specified metric.
  name: Datapoints
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-metric-statistics-output-schema.json
slug: cloudwatch-get-metric-statistics-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMetricStatisticsOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"A label for the specified metric.\"\n    },\n    \"Datapoints\": {\n      \"type\": \"array\",\n      \"description\": \"The data points for the specified metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-statistics-output-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetMetricStatisticsOutput
---
