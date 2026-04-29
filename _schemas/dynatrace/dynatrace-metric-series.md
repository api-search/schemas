---
description: A time-series data series returned by the Dynatrace Metrics API v2 query endpoint, representing metric values for a specific set of dimensions over a time range.
layout: schema
name: Dynatrace Metric Series
properties_list:
- description: The metric key with applied transformations, e.g. builtin:host.cpu.usage:avg. This key identifies the metric and any selector transformations that were applied during the query.
  name: metricId
  type: string
- description: Array of time series, one per unique dimension combination. Each item represents a distinct set of dimension values (e.g., a specific host or service) with its corresponding timestamps and metric valu
  name: data
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-metric-series-schema.json
slug: dynatrace-metric-series
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.dynatrace.com/schemas/metrics/metric-series.json\",\n  \"title\": \"Dynatrace Metric Series\",\n  \"description\": \"A time-series data series returned by the Dynatrace Metrics API v2 query endpoint, representing metric values for a specific set of dimensions over a time range.\",\n  \"type\": \"object\",\n  \"required\": [\"metricId\", \"data\"],\n  \"properties\": {\n    \"metricId\": {\n      \"type\": \"string\",\n      \"description\": \"The metric key with applied transformations, e.g. builtin:host.cpu.usage:avg. This key identifies the metric and any selector transformations that were applied during the query.\",\n      \"examples\": [\n        \"builtin:host.cpu.usage:avg\",\n        \"builtin:service.response.time:percentile(95)\",\n        \"custom.my.metric:sum\"\n      ]\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of time series,\
  \ one per unique dimension combination. Each item represents a distinct set of dimension values (e.g., a specific host or service) with its corresponding timestamps and metric values.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/MetricSeries\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"MetricSeries\": {\n      \"type\": \"object\",\n      \"title\": \"Metric Series\",\n      \"description\": \"A single time series for one unique combination of dimension values. Contains parallel arrays of timestamps and values where each index position corresponds to one data point.\",\n      \"required\": [\"timestamps\", \"values\"],\n      \"properties\": {\n        \"dimensionMap\": {\n          \"type\": \"object\",\n          \"description\": \"Key-value map of dimension names to their values for this series. For example, {\\\"host\\\": \\\"web-01\\\", \\\"environment\\\": \\\"production\\\"}. Provides named access to dimension values.\",\n          \"additionalProperties\": {\n        \
  \    \"type\": \"string\"\n          },\n          \"examples\": [\n            {\"host\": \"web-01\", \"environment\": \"production\"},\n            {\"dt.entity.service\": \"SERVICE-ABCDEF1234567890\"}\n          ]\n        },\n        \"dimensions\": {\n          \"type\": \"array\",\n          \"description\": \"Ordered list of dimension values matching the metric's dimension definitions. The order corresponds to the dimensionDefinitions returned in the metric descriptor. Use dimensionMap for named access.\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"examples\": [\n            [\"web-01\", \"production\"],\n            [\"SERVICE-ABCDEF1234567890\"]\n          ]\n        },\n        \"timestamps\": {\n          \"type\": \"array\",\n          \"description\": \"Unix timestamps in milliseconds for each data point in the series. Each timestamp marks the start of the aggregation window for the corresponding value. Aligns one-to-one with the values\
  \ array.\",\n          \"items\": {\n            \"type\": \"integer\",\n            \"description\": \"Unix timestamp in milliseconds\",\n            \"minimum\": 0\n          },\n          \"examples\": [\n            [1609459200000, 1609462800000, 1609466400000]\n          ]\n        },\n        \"values\": {\n          \"type\": \"array\",\n          \"description\": \"Metric values corresponding to each timestamp. A null value indicates no data was available or recorded for that time slot (a gap in the time series). The array length always matches the timestamps array length.\",\n          \"items\": {\n            \"type\": [\"number\", \"null\"],\n            \"description\": \"The metric value for this time slot. Null indicates no data for the corresponding timestamp.\"\n          },\n          \"examples\": [\n            [45.2, 67.8, null, 51.3],\n            [250.0, 310.5, 289.0]\n          ]\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-metric-series-schema.json
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
title: Dynatrace Metric Series
---
