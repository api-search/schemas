---
description: Encapsulates the statistical data that CloudWatch computes from metric data.
layout: schema
name: Datapoint
properties_list:
- description: The time stamp used for the data point.
  name: Timestamp
  type: string
- description: The number of metric values that contributed to the aggregate value of this data point.
  name: SampleCount
  type: number
- description: The average of the metric values that correspond to the data point.
  name: Average
  type: number
- description: The sum of the metric values for the data point.
  name: Sum
  type: number
- description: The minimum metric value for the data point.
  name: Minimum
  type: number
- description: The maximum metric value for the data point.
  name: Maximum
  type: number
- description: The percentile statistic for the data point.
  name: ExtendedStatistics
  type: object
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-datapoint-schema.json
slug: cloudwatch-datapoint
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Datapoint\",\n  \"type\": \"object\",\n  \"description\": \"Encapsulates the statistical data that CloudWatch computes from metric data.\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The time stamp used for the data point.\"\n    },\n    \"SampleCount\": {\n      \"type\": \"number\",\n      \"description\": \"The number of metric values that contributed to the aggregate value of this data point.\"\n    },\n    \"Average\": {\n      \"type\": \"number\",\n      \"description\": \"The average of the metric values that correspond to the data point.\"\n    },\n    \"Sum\": {\n      \"type\": \"number\",\n      \"description\": \"The sum of the metric values for the data point.\"\n    },\n    \"Minimum\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum metric value for the data point.\"\n    },\n    \"Maximum\": {\n    \
  \  \"type\": \"number\",\n      \"description\": \"The maximum metric value for the data point.\"\n    },\n    \"ExtendedStatistics\": {\n      \"type\": \"object\",\n      \"description\": \"The percentile statistic for the data point.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-datapoint-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: Datapoint
---
