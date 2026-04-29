---
description: The default aggregation setting for the metric.
layout: schema
name: MetricDefaultAggregation
properties_list:
- description: The aggregation type to apply when no aggregation is specified in the query. For example, avg, sum, or max.
  name: type
  type: string
- description: The parameter for the aggregation type, used for percentile aggregation to specify the percentile value (e.g., 95).
  name: parameter
  type: number
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-metrics-v2-metric-default-aggregation-schema.json
slug: dynatrace-metrics-v2-metric-default-aggregation
source_filename: dynatrace-metrics-v2-metric-default-aggregation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The default aggregation setting for the metric.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The aggregation type to apply when no aggregation is specified in the query. For example, avg, sum, or max.\",\n      \"example\": \"min\",\n      \"enum\": [\n        \"min\",\n        \"max\",\n        \"sum\",\n        \"count\",\n        \"avg\",\n        \"median\",\n        \"percentile\"\n      ]\n    },\n    \"parameter\": {\n      \"type\": \"number\",\n      \"description\": \"The parameter for the aggregation type, used for percentile aggregation to specify the percentile value (e.g., 95).\",\n      \"format\": \"double\",\n      \"example\": 87.5\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDefaultAggregation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-metrics-v2-metric-default-aggregation-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: MetricDefaultAggregation
---
