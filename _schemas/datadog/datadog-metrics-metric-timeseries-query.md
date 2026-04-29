---
description: Request body for querying timeseries metric data
layout: schema
name: MetricTimeseriesQuery
properties_list:
- description: The query data object containing type and attributes
  name: data
  type: object
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-timeseries-query-schema.json
slug: datadog-metrics-metric-timeseries-query
source_filename: datadog-metrics-metric-timeseries-query-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-timeseries-query-schema.json\",\n  \"title\": \"MetricTimeseriesQuery\",\n  \"description\": \"Request body for querying timeseries metric data\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The query data object containing type and attributes\",\n      \"required\": [\n        \"type\",\n        \"attributes\"\n      ],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The type identifier for the query request\",\n          \"enum\": [\n            \"timeseries_request\"\n          ]\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"description\": \"The query attributes including formulas, queries, and time range\",\n   \
  \       \"required\": [\n            \"from\",\n            \"to\",\n            \"queries\"\n          ],\n          \"properties\": {\n            \"from\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\",\n              \"description\": \"Unix timestamp in milliseconds for the start of the query time range\"\n            },\n            \"to\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\",\n              \"description\": \"Unix timestamp in milliseconds for the end of the query time range\"\n            },\n            \"interval\": {\n              \"type\": \"integer\",\n              \"format\": \"int64\",\n              \"description\": \"The granularity (in milliseconds) for returned data points\"\n            },\n            \"queries\": {\n              \"type\": \"array\",\n              \"description\": \"List of metric queries to evaluate\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/MetricQueryDefinition\"\
  \n              }\n            },\n            \"formulas\": {\n              \"type\": \"array\",\n              \"description\": \"List of formula expressions combining the defined queries\",\n              \"items\": {\n                \"$ref\": \"#/components/schemas/QueryFormula\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-timeseries-query-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricTimeseriesQuery
---
