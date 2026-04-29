---
description: A time series of metric data points for a specific metric type on an SAP HANA Cloud service instance.
layout: schema
name: MetricSeries
properties_list:
- description: The type of metric (e.g., cpu_usage, memory_used, disk_used, active_connections).
  name: metricType
  type: string
- description: The unit of measurement (e.g., percent, bytes, count).
  name: unit
  type: string
- description: The time-ordered list of metric data points.
  name: dataPoints
  type: array
provider_name: SAP HANA
provider_slug: sap-hana
schema_file: json-schema/sap-hana-cloud-rest-metric-series-schema.json
slug: sap-hana-cloud-rest-metric-series
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MetricSeries\",\n  \"type\": \"object\",\n  \"description\": \"A time series of metric data points for a specific metric type on an SAP HANA Cloud service instance.\",\n  \"properties\": {\n    \"metricType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of metric (e.g., cpu_usage, memory_used, disk_used, active_connections).\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement (e.g., percent, bytes, count).\"\n    },\n    \"dataPoints\": {\n      \"type\": \"array\",\n      \"description\": \"The time-ordered list of metric data points.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap-hana/refs/heads/main/json-schema/sap-hana-cloud-rest-metric-series-schema.json
tags:
- Analytics
- Cloud
- Database
- Enterprise
- In-Memory
title: MetricSeries
---
