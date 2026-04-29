---
description: ''
layout: schema
name: DescribeAlarmsForMetricInput
properties_list:
- description: The name of the metric.
  name: MetricName
  type: string
- description: The namespace of the metric.
  name: Namespace
  type: string
- description: The percentile statistic for the metric.
  name: ExtendedStatistic
  type: string
- description: The dimensions associated with the metric.
  name: Dimensions
  type: array
- description: The period, in seconds, over which the statistic is applied.
  name: Period
  type: integer
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-describe-alarms-for-metric-input-schema.json
slug: cloudwatch-describe-alarms-for-metric-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DescribeAlarmsForMetricInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MetricName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metric.\"\n    },\n    \"Namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The namespace of the metric.\"\n    },\n    \"ExtendedStatistic\": {\n      \"type\": \"string\",\n      \"description\": \"The percentile statistic for the metric.\"\n    },\n    \"Dimensions\": {\n      \"type\": \"array\",\n      \"description\": \"The dimensions associated with the metric.\"\n    },\n    \"Period\": {\n      \"type\": \"integer\",\n      \"description\": \"The period, in seconds, over which the statistic is applied.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-describe-alarms-for-metric-input-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: DescribeAlarmsForMetricInput
---
