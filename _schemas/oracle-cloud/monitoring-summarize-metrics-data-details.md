---
description: Details for summarizing metrics data.
layout: schema
name: SummarizeMetricsDataDetails
properties_list:
- description: The metric namespace.
  name: namespace
  type: string
- description: The Monitoring Query Language expression.
  name: query
  type: string
- description: Start of the time range.
  name: startTime
  type: string
- description: End of the time range.
  name: endTime
  type: string
- description: The time interval for aggregation.
  name: resolution
  type: string
provider_name: Oracle Cloud Infrastructure
provider_slug: oracle-cloud
schema_file: json-schema/monitoring-summarize-metrics-data-details-schema.json
slug: monitoring-summarize-metrics-data-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-summarize-metrics-data-details-schema.json\",\n  \"title\": \"SummarizeMetricsDataDetails\",\n  \"description\": \"Details for summarizing metrics data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"namespace\",\n    \"query\"\n  ],\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"string\",\n      \"description\": \"The metric namespace.\",\n      \"example\": \"oci_computeagent\"\n    },\n    \"query\": {\n      \"type\": \"string\",\n      \"description\": \"The Monitoring Query Language expression.\",\n      \"example\": \"CpuUtilization[1m].mean()\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"description\": \"Start of the time range.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"endTime\": {\n  \
  \    \"type\": \"string\",\n      \"description\": \"End of the time range.\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-18T10:30:00Z\"\n    },\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"The time interval for aggregation.\",\n      \"example\": \"1m\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oracle-cloud/refs/heads/main/json-schema/monitoring-summarize-metrics-data-details-schema.json
tags:
- Cloud Computing
- Enterprise Cloud
- Infrastructure as a Service
- Oracle
- Platform as a Service
title: SummarizeMetricsDataDetails
---
