---
description: Encapsulates the information sent to either create a metric or add new values to be aggregated into an existing metric.
layout: schema
name: MetricDatum
properties_list:
- description: The name of the metric.
  name: MetricName
  type: string
- description: The dimensions associated with the metric.
  name: Dimensions
  type: array
- description: The time the metric data was received, expressed as the number of milliseconds since Jan 1, 1970 00:00:00 UTC.
  name: Timestamp
  type: string
- description: The value for the metric. Although the parameter accepts numbers of type Double, CloudWatch rejects values that are either too small or too large.
  name: Value
  type: number
- description: Array of numbers representing the values for the metric during the period.
  name: Values
  type: array
- description: Array of numbers that is used along with the Values array.
  name: Counts
  type: array
- description: Valid values are 1 and 60. Setting this to 1 specifies this metric as a high-resolution metric.
  name: StorageResolution
  type: integer
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-datum-schema.json
slug: cloudwatch-metric-datum
source_filename: cloudwatch-metric-datum-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDatum\",\n  \"type\": \"object\",\n  \"description\": \"Encapsulates the information sent to either create a metric or add new values to be aggregated into an existing metric.\",\n  \"properties\": {\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions associated with the metric.\"\n    },\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The time the metric data was received, expressed as the number of milliseconds since Jan 1, 1970 00:00:00 UTC.\"\n    },\n    \"Value\": {\n      \"type\": \"number\",\n      \"description\": \"The value for the metric. Although the parameter accepts numbers of type Double, CloudWatch rejects values that are either too small or too large.\"\n    },\n    \"Values\": {\n      \"\
  type\": \"array\",\n      \"description\": \"Array of numbers representing the values for the metric during the period.\"\n    },\n    \"Counts\": {\n      \"type\": \"array\",\n      \"description\": \"Array of numbers that is used along with the Values array.\"\n    },\n    \"StorageResolution\": {\n      \"type\": \"integer\",\n      \"description\": \"Valid values are 1 and 60. Setting this to 1 specifies this metric as a high-resolution metric.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-datum-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricDatum
---
