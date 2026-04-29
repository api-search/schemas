---
description: A GetMetricData call returns an array of MetricDataResult structures.
layout: schema
name: MetricDataResult
properties_list:
- description: The short name you specified to represent this metric.
  name: Id
  type: string
- description: The human-readable label associated with the data.
  name: Label
  type: string
- description: The timestamps for the data points, formatted in Unix epoch time.
  name: Timestamps
  type: array
- description: The data points for the metric corresponding to Timestamps.
  name: Values
  type: array
- description: The status of the returned data.
  name: StatusCode
  type: string
- description: A list of messages with additional information about the data returned.
  name: Messages
  type: array
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-data-result-schema.json
slug: cloudwatch-metric-data-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataResult\",\n  \"type\": \"object\",\n  \"description\": \"A GetMetricData call returns an array of MetricDataResult structures.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The short name you specified to represent this metric.\"\n    },\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable label associated with the data.\"\n    },\n    \"Timestamps\": {\n      \"type\": \"array\",\n      \"description\": \"The timestamps for the data points, formatted in Unix epoch time.\"\n    },\n    \"Values\": {\n      \"type\": \"array\",\n      \"description\": \"The data points for the metric corresponding to Timestamps.\"\n    },\n    \"StatusCode\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the returned data.\"\n    },\n    \"Messages\": {\n      \"type\": \"array\",\n      \"\
  description\": \"A list of messages with additional information about the data returned.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-data-result-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricDataResult
---
