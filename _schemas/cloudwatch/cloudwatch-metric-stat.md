---
description: This structure defines the metric to be returned, along with the statistics, period, and units.
layout: schema
name: MetricStat
properties_list:
- description: The granularity, in seconds, of the returned data points.
  name: Period
  type: integer
- description: The statistic to return. It can include any CloudWatch statistic or extended statistic.
  name: Stat
  type: string
provider_name: AWS CloudWatch
provider_slug: cloudwatch
schema_file: json-schema/cloudwatch-metric-stat-schema.json
slug: cloudwatch-metric-stat
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricStat\",\n  \"type\": \"object\",\n  \"description\": \"This structure defines the metric to be returned, along with the statistics, period, and units.\",\n  \"properties\": {\n    \"Period\": {\n      \"type\": \"integer\",\n      \"description\": \"The granularity, in seconds, of the returned data points.\"\n    },\n    \"Stat\": {\n      \"type\": \"string\",\n      \"description\": \"The statistic to return. It can include any CloudWatch statistic or extended statistic.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cloudwatch/refs/heads/main/json-schema/cloudwatch-metric-stat-schema.json
tags:
- Alarms
- Aws
- Dashboards
- Logs
- Metrics
- Monitoring
- Observability
title: MetricStat
---
