---
description: This structure is used in both GetMetricData and PutMetricAlarm. The supported use of this structure is different for those two operations.
layout: schema
name: MetricDataQuery
properties_list:
- description: A short name used to tie this object to the results in the response.
  name: Id
  type: string
- description: This field can contain a Metrics Insights query, or a metric math expression.
  name: Expression
  type: string
- description: A human-readable label for this metric or expression.
  name: Label
  type: string
- description: When used in GetMetricData, this option indicates whether to return the timestamps and raw data values of this metric.
  name: ReturnData
  type: boolean
- description: The granularity, in seconds, of the returned data points.
  name: Period
  type: integer
- description: The ID of the account where the metrics are located.
  name: AccountId
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-data-query-schema.json
slug: cloudwatch-metric-data-query
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataQuery\",\n  \"type\": \"object\",\n  \"description\": \"This structure is used in both GetMetricData and PutMetricAlarm. The supported use of this structure is different for those two operations.\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"A short name used to tie this object to the results in the response.\"\n    },\n    \"Expression\": {\n      \"type\": \"string\",\n      \"description\": \"This field can contain a Metrics Insights query, or a metric math expression.\"\n    },\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable label for this metric or expression.\"\n    },\n    \"ReturnData\": {\n      \"type\": \"boolean\",\n      \"description\": \"When used in GetMetricData, this option indicates whether to return the timestamps and raw data values of this metric.\"\n    },\n    \"Period\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"The granularity, in seconds, of the returned data points.\"\n    },\n    \"AccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the account where the metrics are located.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-data-query-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricDataQuery
---
