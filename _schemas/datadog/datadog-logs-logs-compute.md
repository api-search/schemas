---
description: A computation to perform over the filtered log set
layout: schema
name: LogsCompute
properties_list:
- description: The type of aggregation to compute over log events
  name: aggregation
  type: string
- description: The log attribute to aggregate (required for all aggregations except count)
  name: metric
  type: string
- description: Whether this is a total aggregation or a timeseries
  name: type
  type: string
- description: The time interval for timeseries computations (e.g., 1m, 1h, 1d)
  name: interval
  type: string
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-logs-logs-compute-schema.json
slug: datadog-logs-logs-compute
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-compute-schema.json\",\n  \"title\": \"LogsCompute\",\n  \"description\": \"A computation to perform over the filtered log set\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregation\": {\n      \"type\": \"string\",\n      \"description\": \"The type of aggregation to compute over log events\",\n      \"enum\": [\n        \"count\",\n        \"cardinality\",\n        \"pc75\",\n        \"pc90\",\n        \"pc95\",\n        \"pc98\",\n        \"pc99\",\n        \"sum\",\n        \"avg\",\n        \"min\",\n        \"max\"\n      ],\n      \"example\": \"count\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"The log attribute to aggregate (required for all aggregations except count)\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"Whether this is a total aggregation or a timeseries\",\n      \"enum\": [\n        \"total\",\n        \"timeseries\"\n      ],\n      \"example\": \"total\"\n    },\n    \"interval\": {\n      \"type\": \"string\",\n      \"description\": \"The time interval for timeseries computations (e.g., 1m, 1h, 1d)\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"aggregation\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-logs-logs-compute-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: LogsCompute
---
