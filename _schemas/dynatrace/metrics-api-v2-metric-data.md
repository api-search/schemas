---
description: The result of a metric query, containing time-series data for each requested metric and dimension combination.
layout: schema
name: MetricData
properties_list:
- description: The resolution of the data points in the response. For example, 1h means each data point represents one hour of data.
  name: resolution
  type: string
- description: The cursor for the next page of results if the response is paginated. Null if all results are returned.
  name: nextPageKey
  type: string
- description: The total number of data series in the result.
  name: totalCount
  type: integer
- description: The list of metric series collections, one per metric key matched by the selector.
  name: result
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/metrics-api-v2-metric-data-schema.json
slug: metrics-api-v2-metric-data
source_filename: metrics-api-v2-metric-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-data-schema.json\",\n  \"title\": \"MetricData\",\n  \"description\": \"The result of a metric query, containing time-series data for each requested metric and dimension combination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"The resolution of the data points in the response. For example, 1h means each data point represents one hour of data.\",\n      \"example\": \"example-value\"\n    },\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results if the response is paginated. Null if all results are returned.\",\n      \"nullable\": true,\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"\
  format\": \"int64\",\n      \"description\": \"The total number of data series in the result.\",\n      \"example\": 500\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"The list of metric series collections, one per metric key matched by the selector.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricSeriesCollection\"\n      },\n      \"example\": [\n        {\n          \"metricId\": \"abc123\",\n          \"data\": [\n            {}\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-data-schema.json
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
title: MetricData
---
