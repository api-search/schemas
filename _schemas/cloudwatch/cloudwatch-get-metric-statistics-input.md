---
description: ''
layout: schema
name: GetMetricStatisticsInput
properties_list:
- description: The namespace of the metric.
  name: Namespace
  type: string
- description: The name of the metric.
  name: MetricName
  type: string
- description: The dimensions to filter the metric.
  name: Dimensions
  type: array
- description: The time stamp that determines the first data point to return.
  name: StartTime
  type: string
- description: The time stamp that determines the last data point to return.
  name: EndTime
  type: string
- description: The granularity, in seconds, of the returned data points.
  name: Period
  type: integer
- description: The metric statistics.
  name: Statistics
  type: array
- description: The percentile statistics.
  name: ExtendedStatistics
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-get-metric-statistics-input-schema.json
slug: cloudwatch-get-metric-statistics-input
source_filename: cloudwatch-get-metric-statistics-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetMetricStatisticsInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric.\"\n    },\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions to filter the metric.\"\n    },\n    \"StartTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp that determines the first data point to return.\"\n    },\n    \"EndTime\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp that determines the last data point to return.\"\n    },\n    \"Period\": {\n      \"type\": \"integer\",\n      \"description\": \"The granularity, in seconds, of the returned data points.\"\n    },\n    \"Statistics\": {\n      \"type\"\
  : \"array\",\n      \"description\": \"The metric statistics.\"\n    },\n    \"ExtendedStatistics\": {\n      \"type\": \"array\",\n      \"description\": \"The percentile statistics.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-get-metric-statistics-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: GetMetricStatisticsInput
---
