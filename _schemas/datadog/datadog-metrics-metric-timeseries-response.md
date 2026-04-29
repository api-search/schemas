---
description: Response containing timeseries metric data for the requested queries
layout: schema
name: MetricTimeseriesResponse
properties_list:
- description: The response data object
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-timeseries-response-schema.json
slug: datadog-metrics-metric-timeseries-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-timeseries-response-schema.json\",\n  \"title\": \"MetricTimeseriesResponse\",\n  \"description\": \"Response containing timeseries metric data for the requested queries\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The response data object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type identifier for the response\"\n        },\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"A unique identifier for this response\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"The response attributes containing timeseries results\",\n          \"properties\": {\n       \
  \     \"times\": {\n              \"type\": \"array\",\n              \"description\": \"Array of Unix timestamps in milliseconds for each data point\",\n              \"items\": {\n                \"type\": \"integer\",\n                \"format\": \"int64\"\n              }\n            },\n            \"series\": {\n              \"type\": \"array\",\n              \"description\": \"List of timeseries results, one per query formula\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/TimeseriesResult\"\n              }\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-timeseries-response-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricTimeseriesResponse
---
