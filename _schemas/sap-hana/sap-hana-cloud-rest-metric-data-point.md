---
description: A single metric data point at a specific timestamp.
layout: schema
name: MetricDataPoint
properties_list:
- description: ISO 8601 timestamp for the data point.
  name: timestamp
  type: string
- description: The metric value at the given timestamp.
  name: value
  type: number
- description: The minimum value observed during the aggregation interval.
  name: min
  type: number
- description: The maximum value observed during the aggregation interval.
  name: max
  type: number
- description: The average value observed during the aggregation interval.
  name: avg
  type: number
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-metric-data-point-schema.json
slug: sap-hana-cloud-rest-metric-data-point
source_filename: sap-hana-cloud-rest-metric-data-point-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricDataPoint\",\n  \"type\": \"object\",\n  \"description\": \"A single metric data point at a specific timestamp.\",\n  \"properties\": {\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"ISO 8601 timestamp for the data point.\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"The metric value at the given timestamp.\"\n    },\n    \"min\": {\n      \"type\": \"number\",\n      \"description\": \"The minimum value observed during the aggregation interval.\"\n    },\n    \"max\": {\n      \"type\": \"number\",\n      \"description\": \"The maximum value observed during the aggregation interval.\"\n    },\n    \"avg\": {\n      \"type\": \"number\",\n      \"description\": \"The average value observed during the aggregation interval.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-metric-data-point-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: MetricDataPoint
---
