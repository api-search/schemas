---
description: A single timeseries result for a query formula
layout: schema
name: TimeseriesResult
properties_list:
- description: Index of the query or formula that produced this result
  name: query_index
  type: integer
- description: Unit information for the metric values in this series
  name: unit
  type: array
- description: The tag key:value pairs that identify this series within a group-by
  name: group_tags
  type: array
- description: The numeric values at each timestamp
  name: values
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-timeseries-result-schema.json
slug: datadog-metrics-timeseries-result
source_filename: datadog-metrics-timeseries-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-timeseries-result-schema.json\",\n  \"title\": \"TimeseriesResult\",\n  \"description\": \"A single timeseries result for a query formula\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"query_index\": {\n      \"type\": \"integer\",\n      \"description\": \"Index of the query or formula that produced this result\",\n      \"example\": 42\n    },\n    \"unit\": {\n      \"type\": \"array\",\n      \"description\": \"Unit information for the metric values in this series\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"family\": {\n            \"type\": \"string\",\n            \"description\": \"The unit family (e.g., time, bytes, percent)\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"\
  The unit name (e.g., second, byte, percent)\"\n          }\n        }\n      }\n    },\n    \"group_tags\": {\n      \"type\": \"array\",\n      \"description\": \"The tag key:value pairs that identify this series within a group-by\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"description\": \"The numeric values at each timestamp\",\n      \"items\": {\n        \"type\": \"number\",\n        \"format\": \"double\",\n        \"nullable\": true\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-timeseries-result-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: TimeseriesResult
---
