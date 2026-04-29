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
schema_file: json-schema/dynatrace-metrics-v2-metric-data-schema.json
slug: dynatrace-metrics-v2-metric-data
source_filename: dynatrace-metrics-v2-metric-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result of a metric query, containing time-series data for each requested metric and dimension combination.\",\n  \"properties\": {\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"The resolution of the data points in the response. For example, 1h means each data point represents one hour of data.\",\n      \"example\": \"example-value\"\n    },\n    \"nextPageKey\": {\n      \"type\": \"string\",\n      \"description\": \"The cursor for the next page of results if the response is paginated. Null if all results are returned.\",\n      \"example\": \"example-value\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The total number of data series in the result.\",\n      \"format\": \"int64\",\n      \"example\": 500\n    },\n    \"result\": {\n      \"type\": \"array\",\n      \"description\": \"The list of metric series collections, one per metric key matched\
  \ by the selector.\",\n      \"example\": [\n        {\n          \"metricId\": \"abc123\",\n          \"data\": [\n            {}\n          ]\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A collection of time-series data for a single metric key, containing one series per unique dimension combination.\",\n        \"properties\": {\n          \"metricId\": {\n            \"type\": \"string\",\n            \"description\": \"The metric key for this collection, including any applied transformations.\",\n            \"example\": \"abc123\"\n          },\n          \"data\": {\n            \"type\": \"array\",\n            \"description\": \"The list of individual time series, one per unique combination of dimension values.\",\n            \"example\": [\n              {\n                \"dimensionMap\": {},\n                \"dimensions\": [\n                  {}\n                ],\n                \"timestamps\": [\n               \
  \   {}\n                ],\n                \"values\": [\n                  {}\n                ]\n              }\n            ],\n            \"items\": {\n              \"type\": \"object\",\n              \"description\": \"A single time series representing metric values for a specific combination of dimension values over a time range.\",\n              \"properties\": {\n                \"dimensionMap\": {\n                  \"type\": \"object\",\n                  \"description\": \"A map of dimension names to their values for this specific series. For example, {\\\"host\\\": \\\"web-01\\\", \\\"environment\\\": \\\"production\\\"}.\",\n                  \"example\": {}\n                },\n                \"dimensions\": {\n                  \"type\": \"array\",\n                  \"description\": \"An ordered list of dimension values corresponding to the metric's dimension definitions.\",\n                  \"example\": [\n                    \"example-value\"\n              \
  \    ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"timestamps\": {\n                  \"type\": \"array\",\n                  \"description\": \"Unix timestamps in milliseconds for each data point in the series. Aligns one-to-one with the values array.\",\n                  \"example\": [\n                    1718153645993\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n                },\n                \"values\": {\n                  \"type\": \"array\",\n                  \"description\": \"Metric values corresponding to each timestamp. A null value indicates no data was recorded for that time slot (gap in the data).\",\n                  \"example\": [\n                    \"example-value\"\n                  ],\n                  \"items\": {\n                    \"type\": \"object\"\n                  }\n              \
  \  }\n              },\n              \"required\": [\n                \"timestamps\",\n                \"values\"\n              ]\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricData\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-metrics-v2-metric-data-schema.json
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
