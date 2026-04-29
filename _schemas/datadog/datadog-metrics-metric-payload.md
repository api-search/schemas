---
description: The payload containing one or more metric series to submit
layout: schema
name: MetricPayload
properties_list:
- description: List of metric series to submit in this payload
  name: series
  type: array
provider_name: Datadog
provider_slug: datadog
schema_file: json-schema/datadog-metrics-metric-payload-schema.json
slug: datadog-metrics-metric-payload
source_filename: datadog-metrics-metric-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-payload-schema.json\",\n  \"title\": \"MetricPayload\",\n  \"description\": \"The payload containing one or more metric series to submit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"series\": {\n      \"type\": \"array\",\n      \"description\": \"List of metric series to submit in this payload\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MetricSeries\"\n      }\n    }\n  },\n  \"required\": [\n    \"series\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/datadog/refs/heads/main/json-schema/datadog-metrics-metric-payload-schema.json
tags:
- Analytics
- Dashboards
- Monitoring
- Platform
- T1
- Visualizations
title: MetricPayload
---
