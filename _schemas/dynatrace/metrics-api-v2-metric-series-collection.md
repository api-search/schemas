---
description: A collection of time-series data for a single metric key, containing one series per unique dimension combination.
layout: schema
name: MetricSeriesCollection
properties_list:
- description: The metric key for this collection, including any applied transformations.
  name: metricId
  type: string
- description: The list of individual time series, one per unique combination of dimension values.
  name: data
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/metrics-api-v2-metric-series-collection-schema.json
slug: metrics-api-v2-metric-series-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-series-collection-schema.json\",\n  \"title\": \"MetricSeriesCollection\",\n  \"description\": \"A collection of time-series data for a single metric key, containing one series per unique dimension combination.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricId\": {\n      \"type\": \"string\",\n      \"description\": \"The metric key for this collection, including any applied transformations.\",\n      \"example\": \"abc123\"\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"The list of individual time series, one per unique combination of dimension values.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricSeries\"\n      },\n      \"example\": [\n        {\n          \"dimensionMap\": {},\n          \"dimensions\": [\n  \
  \          {}\n          ],\n          \"timestamps\": [\n            {}\n          ],\n          \"values\": [\n            {}\n          ]\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/metrics-api-v2-metric-series-collection-schema.json
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
title: MetricSeriesCollection
---
